# Luna::is_interface_implemented_by_type

```c++
bool is_interface_implemented_by_type(typeinfo_t type, const Guid &iid)
```

Checks whether the specified type implements the specified interface. 



## Parameters
* *in* **type**

    The type to query. 

* *in* **iid**

    The interface GUID to query. 

## Return value
Returns `true` if the specified type implements the specified interface. Returns `false` otherwise. 

