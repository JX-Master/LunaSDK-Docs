# Luna::is_generic_struct_type

```c++
LUNA_RUNTIME_API bool is_generic_struct_type(typeinfo_t type)
```

Checks whether one type is a generic structure type. 



## Parameters
### type
The type object to check. 

## Return value
Returns `true` if the specified type is a generic structure type. Returns `false` otherwise. 

#### Valid Usage
* `type` must specify one valid type object. 

