# Luna::init_module_dependencies

```c++
RV init_module_dependencies(Name module_name)
```

Initializes all dependency modules for the specified module, but leaves the specified module as uninitialized. You may use this API to perform some pre-init configurations for the module initialize process. 



## Parameters
### module_name
The name of the specified module. 

## Remark
If the specified module is already initialized, this function does nothing and succeeds. 

