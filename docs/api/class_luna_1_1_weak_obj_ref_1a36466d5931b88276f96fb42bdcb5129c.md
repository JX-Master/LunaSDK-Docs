# Luna::WeakObjRef::WeakObjRef

```c++
WeakObjRef(const WeakObjRef &rhs)
```

Constructs one reference by coping the pointer from another reference. 

The weak reference counter of the new boxed object, if not null, will be increased. 

## Parameters
* *in* **rhs**

    The reference to copy from. 

