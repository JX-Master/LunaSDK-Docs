# Luna::copy_construct_type

```c++
LUNA_RUNTIME_API void copy_construct_type(typeinfo_t type, void *dst, void *src)
```

Copy constructs one instance of the specified type. 

## Overview
The construction is performed as follows:* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

