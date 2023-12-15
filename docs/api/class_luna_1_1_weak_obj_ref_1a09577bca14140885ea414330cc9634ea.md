# Luna::WeakObjRef::WeakObjRef

```c++
WeakObjRef(object_t rhs)
```

Constructs one reference by providing the underlying pointer directly. 

## Overview
The weak reference counter of the new boxed object will be increased if the provided pointer is valid. 

## Parameters
### ptr
The pointer to set. 
