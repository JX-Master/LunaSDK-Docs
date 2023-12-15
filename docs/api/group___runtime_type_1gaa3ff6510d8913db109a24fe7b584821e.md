# Luna::is_type_trivially_copy_assignable

```c++
LUNA_RUNTIME_API bool is_type_trivially_copy_assignable(typeinfo_t type)
```

Checks whether one type is a trivially copy assignable type. 

## Overview
One type is trivially copy assignable if:* `type` must specify one valid type object. 

