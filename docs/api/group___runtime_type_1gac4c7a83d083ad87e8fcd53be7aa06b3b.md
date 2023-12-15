# Luna::get_type_by_name

```c++
LUNA_RUNTIME_API typeinfo_t get_type_by_name(const Name &name, const Name &alias=Name())
```

Gets one type by its name. 

## Overview


## Parameters
### name
The name of the type. 

### alias
The alias name of the type. 

## Return value
Returns the type object that matches the name. Returns `nullptr` if no such type is found. 

