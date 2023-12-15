# Luna::destruct_type_range

```c++
LUNA_RUNTIME_API void destruct_type_range(typeinfo_t type, void *data, usize count)
```

Destructs one array of instances of the specified type. 

## Overview
The destruction is performed as follows:* `type` must specify one valid type object and cannot be a generic structure type.

* `data` must specify one valid memory address. 

