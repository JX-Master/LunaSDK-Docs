# Luna::LockGuard::operator=

```c++
LockGuard & operator=(_SpinLock &lock)
```

Replaces the acquired spin lock. 

The prior lock will be released firstly if not released, then the new lock will be acquired. 

## Parameters
* *in* **lock**

    The new spin lock to acquire. 

