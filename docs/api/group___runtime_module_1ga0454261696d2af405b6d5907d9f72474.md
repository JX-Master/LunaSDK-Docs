# Luna::remove_module

```c++
void remove_module(Module *handle)
```

Removes one module from the module system. This function cannot be called when the module is currently initialized. 



## Parameters
* *in* **handle**

    The module description structure pointer of the module to remove. 

## Valid Usage
* `handle` must point to one module that is already registered by [add_module](group___runtime_module_1ga3e78ad26f4e2d0672d7c2742c5ce38ac.md). 

