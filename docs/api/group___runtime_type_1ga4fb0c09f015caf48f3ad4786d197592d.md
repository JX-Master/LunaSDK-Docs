# Luna::get_struct_generic_type

```c++
typeinfo_t get_struct_generic_type(typeinfo_t type)
```

Gets the generic structure type from one generic structure instanced type. 



## Parameters
* *in* **type**

    The type of the generic structure instanced type to query. 

## Return value
Returns the generic structure type that instantiated the generic structure instanced type. Returns `nullptr` if `type` is not a generic structure instanced type. 

## Valid Usage
* `type` must specify one valid type object. 

