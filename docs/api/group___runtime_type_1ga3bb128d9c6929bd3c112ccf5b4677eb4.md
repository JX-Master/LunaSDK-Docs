# Luna::move_assign_type_range

```c++
LUNA_RUNTIME_API void move_assign_type_range(typeinfo_t type, void *dst, void *src, usize count)
```

Move assigns one array of instances of the specified type. 

The assignment is performed as follows:* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

