# Luna::move_assign_type

```c++
LUNA_RUNTIME_API void move_assign_type(typeinfo_t type, void *dst, void *src)
```

Move assigns one instance of the specified type. 

The assignment is performed as follows:* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

