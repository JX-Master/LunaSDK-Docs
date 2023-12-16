# Luna::ObjRef::ObjRef

```c++
ObjRef(ObjRef &&rhs)
```

Constructs one reference by moving the pointer from another reference. 

The reference counter of the new boxed object is not modified. 

## Parameters
* *in* **rhs**

    The reference to move from. This reference will be null after this operation. 

