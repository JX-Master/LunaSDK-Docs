# Luna::init_module

```c++
RV init_module(Module *handle)
```

Initializes the specified module and all dependency modules of the specified module. 



## Parameters
* *in* **handle**

    The module to initialize. 

## Remark
If the specified module is already initialized, this function does nothing and succeeds. 

## Valid Usage
* `handle` must point to one module that is already registered by [add_module](group___runtime_module_1ga3e78ad26f4e2d0672d7c2742c5ce38ac.md). 

