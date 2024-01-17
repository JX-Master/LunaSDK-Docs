# Luna::add_modules

```c++
RV add_modules(Span< Module * > handles)
```

Adds modules to the module system. 



## Parameters
* *in* **handles**

    The module description structure pointers. These pointers shall be unique for every added module, the module system uses these pointers to identify modules. 

## Remark
See remarks of [add_module](group___runtime_module_1ga3e78ad26f4e2d0672d7c2742c5ce38ac.md) for details. 

## Valid Usage
* All module pointers in `handles` must point to valid module instances. 

