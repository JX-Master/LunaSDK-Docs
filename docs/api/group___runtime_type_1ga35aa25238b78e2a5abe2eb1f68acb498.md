# Luna::check_property_attribute

```c++
bool check_property_attribute(typeinfo_t type, const Name &property, const Name &name)
```

Checks whether the attribute of the specified property exists. 



## Parameters
* *in* **type**

    The type object. 

* *in* **property**

    The property name. 

* *in* **name**

    The name of the attribute to check. 

## Return value
Returns `true` if the attribute exists. Returns `false` otherwise. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type.

* `property` must not be empty.

* `name` must not be empty. 

