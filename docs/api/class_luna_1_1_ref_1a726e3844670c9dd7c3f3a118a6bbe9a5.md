# Luna::Ref::Ref

```c++
Ref(const ObjRef &rhs)
```

Constructs one reference by coping the pointer from one typeless reference. 

The assignment will fail if the new reference is null or cannot be casted to `_Ty`. If the assignment fails, this reference will be null after this operation. If the assignment succeeds, The strong reference counter of the new boxed object will be increased. 

## Parameters
* *in* **rhs**

    The reference to copy from. 

