# Luna::get_module_by_name

```c++
Module * get_module_by_name(const Name &name)
```

Gets the module pointer by its name. The module must be registered firstly. 



## Parameters
* *in* **name**

    The name of the module. 

## Return value
Returns the registered module pointer, or `nullptr` if the module is not found. 

