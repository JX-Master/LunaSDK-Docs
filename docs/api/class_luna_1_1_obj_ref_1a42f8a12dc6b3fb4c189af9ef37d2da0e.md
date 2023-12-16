# Luna::ObjRef::ObjRef

```c++
ObjRef(object_t ptr)
```

Constructs one reference by providing the underlying pointer directly. 

The strong reference counter of the new boxed object will be increased if the provided pointer is valid. 

## Parameters
* *in* **ptr**

    The pointer to set. 

