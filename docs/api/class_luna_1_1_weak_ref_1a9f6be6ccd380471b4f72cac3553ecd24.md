# Luna::WeakRef::operator=

```c++
WeakRef & operator=(const WeakRef &rhs)
```

Assigns this reference by coping the pointer from another reference of the same type. 

The weak reference counter of the new boxed object, if not null, will be increased. The weak reference counter of the original boxed object, if not null, will be decreased before assignment. 

## Parameters
### rhs
The reference to copy from. 

## Return value
Returns `*this`. 

