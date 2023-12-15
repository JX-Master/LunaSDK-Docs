# Luna::WeakObjRef::operator bool

```c++
operator bool() const
```

Checks whether this reference is valid. 

## Overview
One weak reference is valid when it is not null, and the boxed object is not expired. 

## Return value
Returns `true` when the reference is valid. Returns `false` otherwise. 

