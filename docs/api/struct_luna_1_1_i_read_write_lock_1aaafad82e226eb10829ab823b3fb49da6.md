# Luna::IReadWriteLock::try_acquire_write

```c++
virtual bool try_acquire_write()=0
```

Tries to acquire one write ownership of the lock. 

## Overview
This operation does not block the current thread, it returns immediately no matter whether the ownership is acquired. 

## Return value
Returns `true` if the ownership is acquired when this function returns. Returns `false` otherwise. 

