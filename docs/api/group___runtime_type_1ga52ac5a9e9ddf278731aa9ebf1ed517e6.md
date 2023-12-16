# Luna::get_type_name

```c++
Name get_type_name(typeinfo_t type, Name *alias=nullptr)
```

Gets the name of the specified type. 



## Parameters
* *in* **type**

    The type object. 

* *out* **alias**

    If not `nullptr`, returns the alias of the type. 

## Return value
Returns the name of the specified type. 

## Valid Usage
* `type` must specify one valid type object. 

