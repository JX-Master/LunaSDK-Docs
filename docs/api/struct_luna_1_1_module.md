# Luna::Module
The module interface that should be implemented by the user. 

```c++
struct Luna::Module
```

## Member functions
* [virtual const c8 * get_name()=0](struct_luna_1_1_module_1ae34a0f761c133b9052bd44d4bdf71271.md)

    Gets one module name. Every module must have one unique name, and the name cannot changed after the module has been registered to the module system. 

* [virtual RV on_register()](struct_luna_1_1_module_1ac10c2b8f5dacaf0065ddc9f571349bb8.md)

    Called when the module is registered to the system for the first time. 

* [virtual RV on_init()](struct_luna_1_1_module_1a32e1234aab1955184ea2d9cdd522a117.md)

    Called when the module is initialized. 

* [virtual void on_close()](struct_luna_1_1_module_1a9eb8253590ebbf23639571ddc290e64a.md)

    Called when the module is closed. 

