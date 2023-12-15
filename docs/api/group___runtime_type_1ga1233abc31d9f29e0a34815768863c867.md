# Luna::get_struct_generic_arguments

```c++
LUNA_RUNTIME_API Span< const typeinfo_t > get_struct_generic_arguments(typeinfo_t type)
```

Gets the generic arguments used to instantiate one generic structure instanced type. 

## Overview


## Parameters
### type
The type to query. 

## Return value
Returns the generic arguments of the type. Returns one empty span if `type` is not a generic structure instanced type. 

#### Valid Usage
* `type` must specify one valid type object. 

