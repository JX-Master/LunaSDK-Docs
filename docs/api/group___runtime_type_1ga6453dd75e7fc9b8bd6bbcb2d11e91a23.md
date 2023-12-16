# Luna::get_type_by_name

```c++
typeinfo_t get_type_by_name(const Name &name, const Name &alias=Name())
```

Gets one type by its name. 



## Parameters
* *in* **name**

    The name of the type. 

* *in* **alias**

    The alias name of the type. 

## Return value
Returns the type object that matches the name. Returns `nullptr` if no such type is found. 

