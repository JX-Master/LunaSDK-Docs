# Luna::check_type_attribute

```c++
LUNA_RUNTIME_API bool check_type_attribute(typeinfo_t type, const Name &name)
```

Checks whether the attribute of the specified type exists. 

## Overview


## Parameters
### type
The type object. 

### name
The name of the attribute to check. 

## Return value
Returns `true` if the attribute exists. Returns `false` otherwise. 

#### Valid Usage
* `type` must specify one valid type object.

* `name` must not be empty. 
