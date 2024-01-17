# Luna::add_dependency_modules

```c++
RV add_dependency_modules(Module *current, Span< Module * > dependencies)
```

Adds one span of modules as the dependency modules of one module. 



## Parameters
* *in* **current**

    The current module that depends on `dependencies`. 

* *in* **dependencies**

    The dependency modules. If these modules are not added, they will be added to the module system firstly. 

## Valid Usage
* `current` must point to one module that is already registered by [add_module](group___runtime_module_1ga3e78ad26f4e2d0672d7c2742c5ce38ac.md).

* All module pointers in `dependencies` must point to valid module instances. 

