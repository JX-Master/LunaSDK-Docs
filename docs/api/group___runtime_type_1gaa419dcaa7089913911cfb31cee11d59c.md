# Luna::remove_property_attribute

```c++
LUNA_RUNTIME_API void remove_property_attribute(typeinfo_t type, const Name &property, const Name &name)
```

Removes one attribute of the specified property. 



## Parameters
### type
The type object. 

### property
The property name. 

### name
The name of the attribute to remove. 

#### Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type.

* `property` must not be empty.

* `name` must not be empty. 

