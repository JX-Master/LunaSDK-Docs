# Luna::construct_type

```c++
LUNA_RUNTIME_API void construct_type(typeinfo_t type, void *data)
```

Constructs one instance of the specified type. 

## Overview
The construction is performed as follows:* `type` must specify one valid type object and cannot be a generic structure type.

* `data` must specify one valid memory address. 

