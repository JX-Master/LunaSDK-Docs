# Module system
## Types
* [Luna::ModuleDesc](struct_luna_1_1_module_desc.md)

    Module description structure. 


* [Luna::StaticRegisterModule](struct_luna_1_1_static_register_module.md)

    One static module registration helper class that registers the specified module when being constructed. 


## Alias types
* [using module_init_func_t =  RV()](group___runtime_module_1ga385723c1d909ba7d4b962c2149f7a8dd.md)

    The function to be called when the module is initialized. 

* [using module_close_func_t =  void(void)](group___runtime_module_1gabe0425f7d9265734d1178c4d8f1a1d93.md)

    The function to be called when the module is closed. 

## Functions
* [void add_module(ModuleDesc *module_desc)](group___runtime_module_1gafae4c028f93e65c9b2d39dd174668ab1.md)

    Adds one module to the Runtime. This function can be called before `Luna::init` is called. 

* [void remove_module(ModuleDesc *module_desc)](group___runtime_module_1gaf0ed963684ff42c6ac9e21f0ab19b7b4.md)

    Removes one module from the Runtime. This function cannot be called when the module is currently initialized. 

* [RV init_module_dependencies(const Name &module_name)](group___runtime_module_1ga287b606ba74f41e0a135cf971d3319e6.md)

    Initializes all dependency modules for the specified module, but leaves the specified module as uninitialized. You may use this API to perform some pre-init configurations for the module initialize process. 

* [RV init_module(const Name &module_name)](group___runtime_module_1ga4ed6386e0eabbe2c844af14c090cbc47.md)

    Initializes the specified module and all dependency modules of the specified module. 

* [RV init_modules()](group___runtime_module_1ga80bb97afacd6ae806dbebf46d966068d.md)

    Initializes all uninitialized modules. 

## Macros
* [LUNA_STATIC_REGISTER_MODULE(_name, _dependencies, _init_func, _close_func)](group___runtime_module_1ga14d0363490b3940dd1edc58edaa9bba6.md)

    Registers one module statically. Define this in one of CPP files of your module. 

