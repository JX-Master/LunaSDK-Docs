# Luna::MutexGuard
A RAII wrapper for one mutex object that releases the mutex automatically when the wrapper is destructed. 

```c++
class Luna::MutexGuard
```

## Functions
* [MutexGuard()](class_luna_1_1_mutex_guard_1a7d8cdf5a9287b37a4456378eeeaa98a1.md)

    Constructs an empty mutex lock. 

* [MutexGuard(IMutex *mtx)](class_luna_1_1_mutex_guard_1aabd102c9bc9b3aba227f1ecad69ad461.md)

    Constructs a mutex lock that locks the specified mutex. 

* [bool locked() const](class_luna_1_1_mutex_guard_1a8b660d2fb225d2dc900e1f7d0b60dadf.md)

    Checks whether this mutex lock is locking one mutex. 

* [void lock(IMutex *mtx)](class_luna_1_1_mutex_guard_1a4fe5a0cd117832d4078647d078196222.md)

    Locks the specified mutex. If there is already one locked mutex, the former mutex will be unlocked firstly. 

* [void unlock()](class_luna_1_1_mutex_guard_1a9278be8203e1c42e2619179882ae4403.md)

    Unlocks the currently locking mutex. If no mutex is currently locked, this function does nothing. 

