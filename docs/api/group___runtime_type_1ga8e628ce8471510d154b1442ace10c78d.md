# Luna::set_property_attribute

```c++
void set_property_attribute(typeinfo_t type, const Name &property, const Name &name, const Variant &value=Variant())
```

Sets one attribute of the specified property. 



## Parameters
* *in* **type**

    The type object. 

* *in* **property**

    The property name. 

* *in* **name**

    The name of the attribute to set. 

* *in* **value**

    The value of the attribute. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type.

* `property` must not be empty.

* `name` must not be empty. 

