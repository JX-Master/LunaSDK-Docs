# Luna::is_type_trivially_destructable

```c++
LUNA_RUNTIME_API bool is_type_trivially_destructable(typeinfo_t type)
```

Checks whether one type is a trivially destructable type. 

One type is trivially destructable if:* `type` must specify one valid type object. 

