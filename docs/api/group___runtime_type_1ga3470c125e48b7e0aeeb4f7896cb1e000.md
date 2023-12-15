# Luna::get_struct_generic_parameter_names

```c++
LUNA_RUNTIME_API Span< const Name > get_struct_generic_parameter_names(typeinfo_t type)
```

Gets the generic parameter names of the specified type. 

## Overview


## Parameters
### type
The type to query. 

## Return value
Returns the generic arguments of the type. Returns one empty span if `type` is not a generic structure type or a generic structure instanced type. 

#### Valid Usage
* `type` must specify one valid type object. 

