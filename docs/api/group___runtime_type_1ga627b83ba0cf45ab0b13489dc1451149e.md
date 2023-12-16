# Luna::set_type_attribute

```c++
void set_type_attribute(typeinfo_t type, const Name &name, const Variant &value=Variant())
```

Sets one attribute of the specified type. 



## Parameters
* *in* **type**

    The type object. 

* *in* **name**

    The name of the attribute to set. 

* *in* **value**

    The value of the attribute. 

## Remark
If `type` specifies one generic type, the attribute will be applied to all instanced types of that generic type. 

## Valid Usage
* `type` must specify one valid type object.

* `name` must not be empty. 

