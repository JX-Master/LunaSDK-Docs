# Luna::get_enum_underlying_type

```c++
typeinfo_t get_enum_underlying_type(typeinfo_t type)
```

Gets the underlying type of the specified enumeration. 



## Parameters
* *in* **type**

    The type to query. 

## Return value
Returns the underlying type of the specified enumeration. Returns `nullptr` if `type` is not an enumeration type. 

## Valid Usage
* `type` must specify one valid type object. 

