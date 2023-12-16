# Luna::ObjRef::operator=

```c++
ObjRef & operator=(object_t rhs)
```

Replaces the underlying pointer of this reference with the given pointer. 

The strong reference counter of the new boxed object will be increased if the provided pointer is valid. The weak reference counter of the original boxed object, if not null, will be decreased before assignment. 

## Parameters
* *in* **rhs**

    The pointer to set. 

## Return value
Returns `*this`. 

