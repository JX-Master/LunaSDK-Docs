# Thread management and synchronization methods
## Classes
* [Luna::IMutex](struct_luna_1_1_i_mutex.md)
* [Luna::MutexGuard](class_luna_1_1_mutex_guard.md)
* [Luna::IReadWriteLock](struct_luna_1_1_i_read_write_lock.md)
* [Luna::ISemaphore](struct_luna_1_1_i_semaphore.md)
* [Luna::ISignal](struct_luna_1_1_i_signal.md)
* [Luna::IThread](struct_luna_1_1_i_thread.md)
## Functions
* [LUNA_RUNTIME_API Ref< IMutex > new_mutex()](group___runtime_thread_1gaee1e0f158ed71c7afce1527e76c4efaf.md)
* [LUNA_RUNTIME_API Ref< IReadWriteLock > new_read_write_lock()](group___runtime_thread_1ga03c08e87246f2dc76f18f1645c9e734d.md)

    Creates one new read write lock. 

* [LUNA_RUNTIME_API Ref< ISemaphore > new_semaphore(i32 initial_count, i32 max_count)](group___runtime_thread_1ga8f5fe21392376f0cb63e03e62a49d73b.md)
* [LUNA_RUNTIME_API Ref< ISignal > new_signal(bool manual_reset)](group___runtime_thread_1ga89646b80a87875a1678378af7041450f.md)

    Create a new signal object. 

* [LUNA_RUNTIME_API u32 get_processors_count()](group___runtime_thread_1ga1437d8723b57ea809873c0c575eb3bc2.md)

    Gets the number of logical processors on the platform. 

* [LUNA_RUNTIME_API Ref< IThread > new_thread(void(*entry_func)(void *params), void *params, const c8 *name=nullptr, u32 stack_size=0)](group___runtime_thread_1ga587d506e50d89f1dbd3eb50a1d9823b8.md)

    Create a new system thread and make it run the callback function. The thread will be closed when the callback function returns. 

* [LUNA_RUNTIME_API IThread * get_current_thread()](group___runtime_thread_1ga18a1eaf3fc4ff341726a06d62c2d1eb5.md)

    Gets the thread object of current running thread. 

* [LUNA_RUNTIME_API IThread * get_main_thread()](group___runtime_thread_1gad33a876fa281df87180c9f54902f4a6a.md)

    Gets the thread object of the main thread. 

* [LUNA_RUNTIME_API void sleep(u32 time_milliseconds)](group___runtime_thread_1gaa95d9cec0a8b41b8247d32e3d86a52f9.md)

    Suspends current thread for a specific period of time. 

* [LUNA_RUNTIME_API void fast_sleep(u32 time_microseconds)](group___runtime_thread_1ga11420d821a7729b18412dae6d9e7152b.md)

    Delays the execution of this thread for a very shout time by yielding this thread several times. 

* [LUNA_RUNTIME_API void yield_current_thread()](group___runtime_thread_1gae5db165e70e5e860edb44d4fcfae8125.md)

    Yields the remain time slice of the current thread and let OS to schedule other threads. 

* [LUNA_RUNTIME_API opaque_t tls_alloc(tls_destructor *destructor=nullptr)](group___runtime_thread_1gaed1656336d293f6fdbce19481fef2916.md)

    Allocates one thread local storage (TLS) slot. 

* [LUNA_RUNTIME_API void tls_free(opaque_t handle)](group___runtime_thread_1ga6b6c4e321ee1494761c429fbcb34ecc5.md)

    Frees the TLS slot allocated by `tls_alloc`. 

* [LUNA_RUNTIME_API void tls_set(opaque_t handle, void *ptr)](group___runtime_thread_1ga381ac43407ca733426c3a3ce19640900.md)

    Set the data bound to the current thread's TLS slot specified by `handle`. 

* [LUNA_RUNTIME_API void * tls_get(opaque_t handle)](group___runtime_thread_1ga6597acf90d9ec80a6195bf673e994174.md)

    Get the value bound to the TLS slot of current thread. 

