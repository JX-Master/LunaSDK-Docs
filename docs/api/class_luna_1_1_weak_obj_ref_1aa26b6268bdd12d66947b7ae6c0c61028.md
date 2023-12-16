# Luna::WeakObjRef::WeakObjRef

```c++
WeakObjRef(const ObjRef &rhs)
```

Constructs one weak reference from one strong reference. 

The weak reference counter of the new boxed object, if not null, will be increased. 

## Parameters
* *in* **rhs**

    The reference to set. 

