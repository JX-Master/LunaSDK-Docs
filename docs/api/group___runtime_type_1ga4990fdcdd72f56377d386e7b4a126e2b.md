# Luna::relocate_type_range

```c++
LUNA_RUNTIME_API void relocate_type_range(typeinfo_t type, void *dst, void *src, usize count)
```

Relocates one array of instances of the specified type. 

## Overview
The relocation is performed as follows:* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

