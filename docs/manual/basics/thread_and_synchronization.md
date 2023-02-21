# Thread and Synchronization

## Threads

```c++
#include <Runtime/Thread.hpp>
```

`new_thread` creates one system-level thread, which is represented by `IThread`. The user can wait for the thread to exit by calling `IThread::wait`, and check whether the thread is exited by calling `IThread::try_wait`. When the last reference to `IThread` is releasing, the system blocks the current thread until the thread quits.

Every thread uses a thread-local variable to record the current thread's handle, which can be retrieved by `get_current_thread`. The main thread's handle is also recorded and can be retrieved from any thread by `get_main_thread`. The user can delay the execution of the current thread by calling `sleep` or `fast_sleep`, the second function is more accurate and will not suspend the current thread if the time specified is smaller than several milliseconds.

The user can call `yield_current_thread` to yield the remain time slice of the current thread and let OS to schedule other threads. This is useful for reducing CPU cycles if the current thread is waiting for another operation to finish by hardware or another thread.

## Thread local storage (TLS)

```c++
#include <Runtime/Thread.hpp>
```

Thread local storage is a set of pointer-sized memory slots that contains unique data for every thread. This can be useful to store thread-local data and is efficient since reading such data does not require synchronization between threads.

Use `tls_alloc` to create a new thread local storage slot. The slot is allocated for every thread in the current process, including threads that are not yet created. Every thread local storage slot may accept an optional destructor function, which will be called to clean up the thread local object when one thread with one non-zero thread local value on the specified slot is exiting.

> The TLS destructor function works only for threads created by `new_thread` on Windows.

`tls_alloc` returns one `opaque_t`-typed handle, which will be used to get the pointer stored in the thread local storage by `tls_get`, and set the pointer stored in the thread local storage by `tls_set`. The stored pointer will be set to `0` by system before it is set by the user for the first time on one particular thread.

`tls_free` frees one thread local storage slot allocated by `tls_alloc`. Note that freeing one TLS slot will not call destructors registered by `tls_alloc`, so make sure to clean up such resources manually.

## Signals

```c++
#include <Runtime/Signal.hpp>
```

Signal (`ISignal`) is a system-level object for execution synchronization between threads. Every signal has two states: triggered  and untriggered. One signal is in untriggered state when it is created. In such state, all threads that wait for the signal will be blocked until the signal is switched to triggered state by calling `ISignal::trigger`. In triggered state, the signal does not block any thread, and all wait calls return immediately.

One signal can be created by `new_signal`. When creating signals, the user need to specify whether the signal should be reset manually. If `manual_reset` is `true`, one `ISignal::trigger` call will release all threads waiting for the signal, and the signal stays in triggered state until `ISignal::reset` is called; if `manual_reset` is `false`, every `ISignal::trigger` call will only release exact one thread waiting for the signal, and the signal will be reset back to untriggered state automatically. The releasing order of threads waiting for the signal is unspecified.

## Mutex

```c++
#include <Runtime/Mutex.hpp>
```

Mutex (`IMutex`) is a system-level object for ensuring exclusive access to one entity. Every mutex have two states: locked and unlocked. One mutex is in unlocked state when it is created. When one mutex is unlocked, the first thread that wants to acquire the mutex succeeds and transfers the mutex to locked state. When one mutex is locked, all other threads that want to acquire the mutex will fail or get blocked until the mutex is released by its owning thread and is transferred into unlocked state. The mutex is recursive, acquiring the mutex multiple times from the same thread is allowed, but the user should release the mutex the same times as she acquires the mutex to finally unlock the mutex.

One mutex can be created by `new_mutex`, and can be acquired by `IMutex::wait` and `IMutex::try_wait`, the second form returns `false` instead of blocking the current thread if failing to acquire the mutex. One mutex can be released by `IMutex::unlock`. The user can use `MutexGuard` helper object to acquire one mutex in one function scope and release it automatically when `MutexGuard` is expired.

## Spin lock

```c++
#include <Runtime/SpinLock.hpp>
```

A spin lock (`SpinLock` or `RecursiveSpinLock`) is a light-weight version of `IMutex` with the following differences:

1. The spin lock is implemented purely in user-mode by C++, while the mutex is implemented by the underlying platform/OS and is usually implemented in kernel-mode as an OS component, which means locking and releasing one spin lock is much faster than locking and releasing one mutex, since the later is usually performed through a system call.
2. The spin lock will never suspend one thread, nor will it yield the time slice of the waiting thread. If one spin lock is already locked, the waiting thread will keep checking (busy-waiting) until it obtains the lock. In the other side, the mutex will usually suspends or yields the current thread if the mutex is already locked to let other threads use the processor. This makes the spin lock suitable for locking the resource for a very short period of time (hundreds or thousands of CPU-cycles), but not suitable if the lock will be obtained for a long time (>100us).
3. Creating one spin lock creation consumes much less memory than creating one mutex (only 4 bytes for non-recursive spin lock). Meanwhile, creating one spin lock does not need to allocate any dynamic memory, just declare and use it, which makes it suitable for embedding into other objects.

One spin lock can be acquired by `lock` and `try_lock`, and can be released by `unlock`. Recursive locking from the same thread is supported only by `RecursiveSpinLock`, not `SpinLock`. The user can use `LockGuard` helper object to acquire one spin lock in one function scope and release it automatically when `LockGuard` is expired. `LockGuard` works for both `SpinLock`  and `RecursiveSpinLock`.

## Semaphore

```c++
#include <Runtime/Semaphore.hpp>
```

Semaphore (`ISemaphore`) is a system-level synchronization object which stores one value between `0` and `max_count`. One semaphore has two states: locked state and unlocked state, it is in unlocked state when the counter value is not `0`, and is in locked state when the counter value is `0`. 



