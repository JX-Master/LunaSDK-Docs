# Luna::ObjRef::ObjRef

```c++
ObjRef(const ObjRef &rhs)
```

Constructs one reference by coping the pointer from another reference. 

The strong reference counter of the new boxed object, if not null, will be increased. 

## Parameters
* *in* **rhs**

    The reference to copy from. 

