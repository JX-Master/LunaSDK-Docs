# Luna::is_type_trivially_relocatable

```c++
LUNA_RUNTIME_API bool is_type_trivially_relocatable(typeinfo_t type)
```

Checks whether one type is a trivially relocatable type. 

One type is trivially relocatable if:* `type` must specify one valid type object. 

