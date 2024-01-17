# Module system
## Types
* [Luna::Module](struct_luna_1_1_module.md)

    The module interface that should be implemented by the user. 


## Functions
* [RV add_module(Module *handle)](group___runtime_module_1ga3e78ad26f4e2d0672d7c2742c5ce38ac.md)

    Adds one module to the module system. If this module is already added, this function does nothing. 

* [RV add_modules(Span< Module * > handles)](group___runtime_module_1ga5a2fcd063c9ade4a20ee2287aab86df6.md)

    Adds modules to the module system. 

* [void remove_module(Module *handle)](group___runtime_module_1ga0454261696d2af405b6d5907d9f72474.md)

    Removes one module from the module system. This function cannot be called when the module is currently initialized. 

* [RV add_dependency_module(Module *current, Module *dependency)](group___runtime_module_1ga5263a9221a92f47e34ebf717f461f36d.md)

    Adds one module as the dependency module of one module. This is usually called in module registration callback. 

* [RV add_dependency_modules(Module *current, Span< Module * > dependencies)](group___runtime_module_1ga0c427695ed3120dd5a1ee5f11d969ee7.md)

    Adds one span of modules as the dependency modules of one module. 

* [Module * get_module_by_name(const Name &name)](group___runtime_module_1ga91d7dc2f74ec72bea967b3fbadad1c59.md)

    Gets the module pointer by its name. The module must be registered firstly. 

* [RV init_module_dependencies(Module *handle)](group___runtime_module_1gaee2ac8ff649352e92a50880f9e0e2a5d.md)

    Initializes all dependency modules for the specified module, but leaves the specified module as uninitialized. You may use this API to perform some pre-init configurations for the module initialize process. 

* [RV init_module(Module *handle)](group___runtime_module_1ga54cef34b7967aad16e0da8253fda317e.md)

    Initializes the specified module and all dependency modules of the specified module. 

* [RV init_modules()](group___runtime_module_1ga80bb97afacd6ae806dbebf46d966068d.md)

    Initializes all uninitialized modules. 

