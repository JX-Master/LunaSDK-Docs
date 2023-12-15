# Luna::WeakObjRef::operator=

```c++
WeakObjRef & operator=(const WeakObjRef &rhs)
```

Assigns this reference by coping the pointer from another reference. 

## Overview
The weak reference counter of the new boxed object, if not null, will be increased. The weak reference counter of the original boxed object, if not null, will be decreased before assignment. 

## Parameters
### rhs
The reference to copy from. 

## Return value
Returns `*this`. 

