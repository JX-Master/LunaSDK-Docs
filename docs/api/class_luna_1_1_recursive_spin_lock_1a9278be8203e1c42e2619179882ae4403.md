# Luna::RecursiveSpinLock::unlock

```c++
void unlock()
```

Unlocks the spin lock. 

If the lock is acquired from the same thread multiple times, the user should call this function the same times as [lock](class_luna_1_1_recursive_spin_lock_1aa81aed607133209dade63a226818224d.md) to finally release the lock. 

