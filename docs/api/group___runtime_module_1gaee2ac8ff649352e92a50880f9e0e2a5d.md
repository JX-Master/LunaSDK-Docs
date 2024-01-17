# Luna::init_module_dependencies

```c++
RV init_module_dependencies(Module *handle)
```

Initializes all dependency modules for the specified module, but leaves the specified module as uninitialized. You may use this API to perform some pre-init configurations for the module initialize process. 



## Parameters
* *in* **handle**

    The module to initialize dependencies. 

## Remark
If the specified module is already initialized, this function does nothing and succeeds. 

## Valid Usage
* `handle` must point to one module that is already registered by [add_module](group___runtime_module_1ga3e78ad26f4e2d0672d7c2742c5ce38ac.md). 

