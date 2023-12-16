# Luna::add_module

```c++
void add_module(ModuleDesc *module_desc)
```

Adds one module to the Runtime. This function can be called before `Luna::init` is called. 

The added module will not be initialized immediately. If the module is added before the Runtime is initialized, they will be initialized when `Luna::init` is called; if the module is added after the Runtime is initialized, they must be initialized by one explicit call to `init_modules`. When `Luna::init` or `init_modules` are called, all dependent modules of the registered module must also be registered.

All modules will be closed by their dependency order when `Luna::close` is called. There is no way to close and remove modules on the fly, since modules are "unmanaged" and it makes the module implementation very complex to do so. You should restart the SDK if you make changes to modules.

## Parameters
* *in* **module_desc**

    The description structure of the module. This structure should be available during the module lifetime. 

