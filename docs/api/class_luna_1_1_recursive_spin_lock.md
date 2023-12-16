# Luna::RecursiveSpinLock
```c++
class Luna::RecursiveSpinLock
```

Similar to [SpinLock](class_luna_1_1_spin_lock.md), but allows the lock to be obtained mutable times from the same thread. The user should release the lock the same times as obtaining the lock to finally release the lock. 

