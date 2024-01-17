# Luna::add_module

```c++
RV add_module(Module *handle)
```

Adds one module to the module system. If this module is already added, this function does nothing. 



## Parameters
* *in* **handle**

    The module description structure pointer. This pointer shall be unique for every added module, the module system uses this pointer to identify the module. 

## Remark
Adding one module to the module system does not initialize the module, the added module must be explicitly initialized using [init_module](group___runtime_module_1ga54cef34b7967aad16e0da8253fda317e.md) or [init_modules](group___runtime_module_1ga80bb97afacd6ae806dbebf46d966068d.md) before it can be used. 

## Valid Usage
* `handle` must point to one valid module instance. 

