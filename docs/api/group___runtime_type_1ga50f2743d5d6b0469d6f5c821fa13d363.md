# Luna::set_enum_instance_value

```c++
void set_enum_instance_value(typeinfo_t type, void *data, i64 value)
```

Sets the enumeration value to the specified mapped value. 

The value is converted to the underlying type of the enumeration before set. 

## Parameters
* *in* **type**

    The type of the instance. 

* *in* **data**

    The instance data. 

* *in* **value**

    The value to set. 

## Valid Usage
* `type` must specify one valid enumeration type object.

* `data` must specify one valid instance whose type is `type`. 

