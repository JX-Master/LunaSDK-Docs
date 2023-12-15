# Luna::get_base_type

```c++
LUNA_RUNTIME_API typeinfo_t get_base_type(typeinfo_t type)
```

Gets the base type of the specified type. 

## Overview


## Parameters
### type
The type to query. 

## Return value
Returns the base type of the specified type. Returns `nullptr` if the specified type is not a structure type, or if the type does not have a base type. 

#### Valid Usage
* `type` must specify one valid type object. 

