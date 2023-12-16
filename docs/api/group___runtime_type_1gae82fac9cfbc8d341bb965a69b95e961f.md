# Luna::get_type_attribute

```c++
Variant get_type_attribute(typeinfo_t type, const Name &name)
```

Gets the attribute of the specified type. 



## Parameters
* *in* **type**

    The type object. 

* *in* **name**

    The name of the attribute to get. 

## Return value
Returns the requested attribute. Returns one null variant if the attribute does not exist. 

## Valid Usage
* `type` must specify one valid type object.

* `name` must not be empty. 

