# Luna::get_enum_instance_value

```c++
i64 get_enum_instance_value(typeinfo_t type, const void *data)
```

Extracts the mapped value of the enumeration, regardless of the underlying type of the enumeration. 



## Parameters
* *in* **type**

    The type of the instance. 

* *in* **data**

    The instance data. 

## Return value
Returns the mapped value of the enumeration converted to signed 64-bit integer. 

## Valid Usage
* `type` must specify one valid enumeration type object.

* `data` must specify one valid instance whose type is `type`. 

