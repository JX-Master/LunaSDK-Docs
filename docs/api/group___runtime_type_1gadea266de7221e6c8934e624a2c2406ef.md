# Luna::check_type_attribute

```c++
bool check_type_attribute(typeinfo_t type, const Name &name)
```

Checks whether the attribute of the specified type exists. 



## Parameters
* *in* **type**

    The type object. 

* *in* **name**

    The name of the attribute to check. 

## Return value
Returns `true` if the attribute exists. Returns `false` otherwise. 

## Valid Usage
* `type` must specify one valid type object.

* `name` must not be empty. 

