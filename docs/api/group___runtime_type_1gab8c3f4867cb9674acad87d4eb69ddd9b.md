# Luna::is_type_trivially_move_assignable

```c++
LUNA_RUNTIME_API bool is_type_trivially_move_assignable(typeinfo_t type)
```

Checks whether one type is a trivially move assignable type. 

## Overview
One type is trivially move assignable if:* `type` must specify one valid type object. 

