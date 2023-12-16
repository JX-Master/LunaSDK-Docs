# Luna::get_property_attribute

```c++
Variant get_property_attribute(typeinfo_t type, const Name &property, const Name &name)
```

Gets the attribute of the specified property. 



## Parameters
* *in* **type**

    The type object. 

* *in* **property**

    The property name. 

* *in* **name**

    The name of the attribute to get. 

## Return value
Returns the requested attribute. Returns one null variant if the attribute does not exist. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type.

* `property` must not be empty.

* `name` must not be empty. 

