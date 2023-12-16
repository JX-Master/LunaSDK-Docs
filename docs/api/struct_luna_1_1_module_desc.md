# Luna::ModuleDesc
Module description structure. 

```c++
struct Luna::ModuleDesc
```

This shall be allocated on static memory and being kept valid during the application lifetime. 

## Member objects
* [c8 reserved[32]](struct_luna_1_1_module_desc_1aa4599232e3e8acf0218788de720c9439.md)

    Used by the Runtime. The user should not change these memory. 

* [const c8* name](struct_luna_1_1_module_desc_1acd5365440f9f8784729838aa744e02c2.md)

    The name of the module. The lifetime of the string should be equal to the lifetime of the module. 

* [const c8* dependencies](struct_luna_1_1_module_desc_1a7d426a60e33a98255d2a2e5f018cff27.md)

    A string that records modules this module depends on. 

* [module_init_func_t* init_func](struct_luna_1_1_module_desc_1ac3c3fcfd83b0007172bb0cd49e4f9b44.md)

    The initialize function of the module. 

* [module_close_func_t* close_func](struct_luna_1_1_module_desc_1a0410004c8e1030f0be3c2c6f692ed685.md)

    The close function of the module. 

