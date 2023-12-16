# Luna::ObjRef::operator=

```c++
ObjRef & operator=(const ObjRef &rhs)
```

Assigns this reference by coping the pointer from another reference. 

The strong reference counter of the new boxed object, if not null, will be increased. The strong reference counter of the original boxed object, if not null, will be decreased before assignment. 

## Parameters
* *in* **rhs**

    The reference to copy from. 

## Return value
Returns `*this`. 

