# Luna::get_property_attributes

```c++
Vector< Name > get_property_attributes(typeinfo_t type, const Name &property)
```

Gets all attributes of the specified property. 



## Parameters
* *in* **type**

    The type object. 

* *in* **property**

    The property name. 

## Return value
Returns one vector that contains attribute names of all attributes of the specified property. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type.

* `property` must not be empty. 

