# Luna::WeakRef::WeakRef

```c++
WeakRef(const Ref< _Ty > &rhs)
```

Constructs one weak reference from one strong reference of the same type. 

The weak reference counter of the new boxed object, if not null, will be increased. 

## Parameters
* *in* **rhs**

    The reference to set. 

