# DLL loading
## Functions
* [LUNA_RUNTIME_API R< opaque_t > load_library(const c8 *path)](group___runtime_d_l_l_1gaf089b17ba5687b844e5ab7233a65a24e.md)

    Loads the specified library to the process's address space. This call may load additional libraries required by the specified library. 

* [LUNA_RUNTIME_API void free_library(opaque_t handle)](group___runtime_d_l_l_1gaeb0bf745d9d2223a5b090a394d686164.md)

    Unloads the specified library. 

* [LUNA_RUNTIME_API R< void * > get_library_function(opaque_t handle, const c8 *symbol)](group___runtime_d_l_l_1ga142f49325d4d28a71112b9b095c51161.md)

    Gets the function address (function pointer) of one function in the library from its symbol name. 

