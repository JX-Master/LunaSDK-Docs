# Luna::get_property_attribute

```c++
LUNA_RUNTIME_API Variant get_property_attribute(typeinfo_t type, const Name &property, const Name &name)
```

Gets the attribute of the specified property. 

## Overview


## Parameters
### type
The type object. 

### property
The property name. 

### name
The name of the attribute to get. 

## Return value
Returns the requested attribute. Returns one null variant if the attribute does not exist. 

#### Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type.

* `property` must not be empty.

* `name` must not be empty. 

