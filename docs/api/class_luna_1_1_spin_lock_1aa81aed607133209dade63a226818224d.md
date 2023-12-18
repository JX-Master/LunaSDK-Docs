# Luna::SpinLock::lock

```c++
void lock()
```

Locks the spin lock. 

This function blocks the current thread until the spin lock is successfully locked. Locking the same spin lock from the same thread twice causes deadlock. Use [RecursiveSpinLock](class_luna_1_1_recursive_spin_lock.md) if you need to lock the same spin lock multiple times from the same thread. 

