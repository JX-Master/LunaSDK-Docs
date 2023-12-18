# Luna::RecursiveSpinLock
Similar to [SpinLock](class_luna_1_1_spin_lock.md), but allows the lock to be obtained mutable times from the same thread. 

```c++
class Luna::RecursiveSpinLock
```

## Member functions
* [RecursiveSpinLock()](class_luna_1_1_recursive_spin_lock_1a80b247570b4d1f083a263804a7f3a877.md)

    Constructs one spin lock. The spin lock is unlocked after creation. 

* [void lock()](class_luna_1_1_recursive_spin_lock_1aa81aed607133209dade63a226818224d.md)

    Locks the spin lock. 

* [bool try_lock()](class_luna_1_1_recursive_spin_lock_1aa24a64f788f142df670c3abc809d32b6.md)

    Tries to lock the spin lock. 

* [void unlock()](class_luna_1_1_recursive_spin_lock_1a9278be8203e1c42e2619179882ae4403.md)

    Unlocks the spin lock. 

