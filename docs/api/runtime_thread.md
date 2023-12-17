# Thread management and synchronization methods
## Classes
* [Luna::IMutex](struct_luna_1_1_i_mutex.md)
* [Luna::MutexGuard](class_luna_1_1_mutex_guard.md)
* [Luna::IReadWriteLock](struct_luna_1_1_i_read_write_lock.md)
* [Luna::ISemaphore](struct_luna_1_1_i_semaphore.md)
* [Luna::ISignal](struct_luna_1_1_i_signal.md)
* [Luna::IThread](struct_luna_1_1_i_thread.md)
## Enumerations
* [Luna::ThreadPriority](group___runtime_thread_1ga80351cf39ce9e4d1d110fb249699db07.md)

    Specifies the thread schedule priority. 

## Functions
* [Ref< IMutex > new_mutex()](group___runtime_thread_1gaaf4b4510b9d6c01a12e3064691d15bdc.md)
* [Ref< IReadWriteLock > new_read_write_lock()](group___runtime_thread_1ga35f290e06f79b34a7a4b72368a88e6b4.md)

    Creates one new read write lock. 

* [Ref< ISemaphore > new_semaphore(i32 initial_count, i32 max_count)](group___runtime_thread_1ga63acf4d842bfddff65e76b2e84524134.md)

    Create a new semaphore object. 

* [Ref< ISignal > new_signal(bool manual_reset)](group___runtime_thread_1ga451437bc4ec31226c33c379fbd7d7a24.md)

    Create a new signal object. 

* [u32 get_processors_count()](group___runtime_thread_1gac8b023e3dd3ae6a46516fa958f2ad7b9.md)

    Gets the number of logical processors on the platform. 

* [Ref< IThread > new_thread(void(*entry_func)(void *params), void *params, const c8 *name=nullptr, u32 stack_size=0)](group___runtime_thread_1gac1aad6a8f99159d07fe287db59c0a318.md)

    Create a new system thread and make it run the callback function. The thread will be closed when the callback function returns. 

* [IThread * get_current_thread()](group___runtime_thread_1ga3ed3f90467bd6b3e0b75a8c1c4562068.md)

    Gets the thread object of current running thread. 

* [IThread * get_main_thread()](group___runtime_thread_1ga1bed2d312e6b95a39bd841d0ededf2b4.md)

    Gets the thread object of the main thread. 

* [void sleep(u32 time_milliseconds)](group___runtime_thread_1ga2ed6b20ac018dd695a1189c68629132a.md)

    Suspends current thread for a specific period of time. 

* [void fast_sleep(u32 time_microseconds)](group___runtime_thread_1gaf28258e2d025ad9da4aa4aa5de2bc339.md)

    Delays the execution of this thread for a very shout time by yielding this thread several times. 

* [void yield_current_thread()](group___runtime_thread_1ga612f977ca8fde0829d4fcf182d4cad00.md)

    Yields the remain time slice of the current thread and let OS to schedule other threads. 

* [opaque_t tls_alloc(tls_destructor *destructor=nullptr)](group___runtime_thread_1ga627934a51a920ff58c694cdb89083fe4.md)

    Allocates one thread local storage (TLS) slot. 

* [void tls_free(opaque_t handle)](group___runtime_thread_1gab3909da8f640a34cf007e78404b41226.md)

    Frees the TLS slot allocated by `tls_alloc`. 

* [void tls_set(opaque_t handle, void *ptr)](group___runtime_thread_1gacb55d976ce0cbe2683bf03116be2d2f2.md)

    Set the data bound to the current thread's TLS slot specified by `handle`. 

* [void * tls_get(opaque_t handle)](group___runtime_thread_1gab310bb1422cf8f1b192bdcc5b3668cc4.md)

    Get the value bound to the TLS slot of current thread. 

