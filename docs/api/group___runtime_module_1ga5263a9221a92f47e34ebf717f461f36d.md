# Luna::add_dependency_module

```c++
RV add_dependency_module(Module *current, Module *dependency)
```

Adds one module as the dependency module of one module. This is usually called in module registration callback. 



## Parameters
* *in* **current**

    The current module that depends on `dependency`. 

* *in* **dependency**

    The dependency module. If this module is not added, it will be added to the module system firstly. 

## Valid Usage
* `current` must point to one module that is already registered by [add_module](group___runtime_module_1ga3e78ad26f4e2d0672d7c2742c5ce38ac.md).

* `dependency` must point to one valid module instance. 

