# Luna::LockGuard
The RAII wrapper that locks the specified lock upon construction, and unlocks the specified lock upon destruction. 

```c++
class Luna::LockGuard
```

This can be used for both [SpinLock](class_luna_1_1_spin_lock.md) and [RecursiveSpinLock](class_luna_1_1_recursive_spin_lock.md)

## Member functions
* [LockGuard(_SpinLock &lock)](class_luna_1_1_lock_guard_1abcad6cffe0c365739483d67cfcd08926.md)

    Constructs one lock guard and acquires the specified lock. 

* [void unlock()](class_luna_1_1_lock_guard_1a9278be8203e1c42e2619179882ae4403.md)

    Releases the acquired spin lock manually. 

* [LockGuard & operator=(_SpinLock &lock)](class_luna_1_1_lock_guard_1a84e43ac52480e865488ca9c31bce7b10.md)

    Replaces the acquired spin lock. 

