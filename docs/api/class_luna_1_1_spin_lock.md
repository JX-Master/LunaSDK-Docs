# Luna::SpinLock
Provides one spin lock that can give one thread exclusive access to one resource in multi-thread environments. 

```c++
class Luna::SpinLock
```

A spin lock is like a light-weight mutex. Both mutex and spin lock are used to give one thread exclusive access to some specific resource, but they have the following differences:1. The spin lock is implemented purely in user-mode by C++, while the mutex is implemented by the underlying platform/OS and is usually implemented in kernel-mode as an OS component, which means locking and releasing one spin lock is much faster than locking and releasing one mutex, since the later is usually performed through a system call.

1. The spin lock will never suspend one thread, nor will it yield the time slice of the waiting thread. If one spin lock is already locked, the waiting thread will keep checking (not_ready-waiting) until it obtains the lock. In the other side, the mutex will usually suspends or yields the current thread if the mutex is already locked to let other threads use the processor. This makes the spin lock suitable for locking the resource for a very short period of time (hundreds or thousands of CPU-cycles), but not suitable if the lock will be obtained for a long time (>100us).

1. Creating one spin lock creation consumes much less memory than creating one mutex (only 4 bytes for non-recursive spin lock). Meanwhile, creating one spin lock does not need to allocate any dynamic memory, which makes it suitable for embedding into other objects. 

## Member functions
* [SpinLock()](class_luna_1_1_spin_lock_1a3175971aac6aef2f7bea331e70d2bdca.md)

    Constructs one spin lock. The spin lock is unlocked after creation. 

* [void lock()](class_luna_1_1_spin_lock_1aa81aed607133209dade63a226818224d.md)

    Locks the spin lock. 

* [bool try_lock()](class_luna_1_1_spin_lock_1aa24a64f788f142df670c3abc809d32b6.md)

    Tries to lock the spin lock. 

* [void unlock()](class_luna_1_1_spin_lock_1a9278be8203e1c42e2619179882ae4403.md)

    Unlocks the spin lock. 

