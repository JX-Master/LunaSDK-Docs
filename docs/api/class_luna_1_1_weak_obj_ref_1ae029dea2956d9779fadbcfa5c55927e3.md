# Luna::WeakObjRef::operator=

```c++
WeakObjRef & operator=(const ObjRef &rhs)
```

Assigns this reference by coping the pointer from one strong reference. 

The weak reference counter of the new boxed object, if not null, will be increased. The weak reference counter of the original boxed object, if not null, will be decreased before assignment. 

## Parameters
### rhs
The reference to set. 

