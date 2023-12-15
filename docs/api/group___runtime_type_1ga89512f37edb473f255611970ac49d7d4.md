# Luna::destruct_type

```c++
LUNA_RUNTIME_API void destruct_type(typeinfo_t type, void *data)
```

Destructs one instance of the specified type. 

## Overview
The destruction is performed as follows:* `type` must specify one valid type object and cannot be a generic structure type.

* `data` must specify one valid memory address. 

