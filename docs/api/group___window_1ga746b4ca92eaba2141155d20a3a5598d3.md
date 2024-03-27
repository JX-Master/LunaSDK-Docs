# Luna::Window::get_name

```c++
const c8 * get_name()
```

Gets the application name. 



## Return value
Returns one string that represents the application name. The string is valid until this module is closed. 

## Remark
The application version is set by filling [StartupParams::name](struct_luna_1_1_window_1_1_startup_params_1acd5365440f9f8784729838aa744e02c2.md) and calling [set_startup_params](group___window_1ga8b673b742e7dd97fdbe78d9cb04ec7d6.md) before Window module is initialized. 

