# Luna::check_property_attribute

```c++
LUNA_RUNTIME_API bool check_property_attribute(typeinfo_t type, const Name &property, const Name &name)
```

Checks whether the attribute of the specified property exists. 

## Overview


## Parameters
### type
The type object. 

### property
The property name. 

### name
The name of the attribute to check. 

## Return value
Returns `true` if the attribute exists. Returns `false` otherwise. 

#### Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type.

* `property` must not be empty.

* `name` must not be empty. 

