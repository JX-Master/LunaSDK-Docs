# Luna::is_type_trivially_move_constructable

```c++
LUNA_RUNTIME_API bool is_type_trivially_move_constructable(typeinfo_t type)
```

Checks whether one type is a trivially move constructable type. 

## Overview
One type is trivially move constructable if:* `type` must specify one valid type object. 

