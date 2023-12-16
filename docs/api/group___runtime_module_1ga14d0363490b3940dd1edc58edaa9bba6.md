# LUNA_STATIC_REGISTER_MODULE

```c++
#define LUNA_STATIC_REGISTER_MODULE(_name, _dependencies, _init_func, _close_func)
```

Registers one module statically. Define this in one of CPP files of your module. 



## Parameters
* *in* **_name**

    The name of the module. *Used* by the **system** to index this module. 

* *in* **_dependencies**

    The dependency modules of this module, written in one string separated by semicolons (";"). 

* *in* **_init_func**

    The module initialization function. 

* *in* **_close_func**

    The module close function. 

## Remark
See docs of [Luna::ModuleDesc](struct_luna_1_1_module_desc.md) for details about every parameter of this macro. 

