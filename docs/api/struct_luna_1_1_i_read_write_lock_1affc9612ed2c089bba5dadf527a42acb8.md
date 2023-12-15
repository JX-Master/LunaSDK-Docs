# Luna::IReadWriteLock::try_acquire_read

```c++
virtual bool try_acquire_read()=0
```

Tries to acquire one read ownership of the lock. 

This operation does not block the current thread, it returns immediately no matter whether the ownership is acquired. 

## Return value
Returns `true` if the ownership is acquired when this function returns. Returns `false` otherwise. 

