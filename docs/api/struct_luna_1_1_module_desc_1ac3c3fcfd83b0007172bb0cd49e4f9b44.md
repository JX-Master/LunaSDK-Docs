# Luna::ModuleDesc::init_func

```c++
module_init_func_t* init_func
```

The initialize function of the module. 

This can be `nullptr`, which behaves the same as returning `RV()` directly. 

