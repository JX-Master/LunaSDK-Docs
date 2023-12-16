# DLL loading
## Functions
* [R< opaque_t > load_library(const c8 *path)](group___runtime_d_l_l_1ga4047beea74e118348cddab00150eb4f8.md)

    Loads the specified library to the process's address space. This call may load additional libraries required by the specified library. 

* [void free_library(opaque_t handle)](group___runtime_d_l_l_1gada1eb355bd34c85c93378ecc592379d3.md)

    Unloads the specified library. 

* [R< void * > get_library_function(opaque_t handle, const c8 *symbol)](group___runtime_d_l_l_1ga71c8be52fc489d33272082e385187ebc.md)

    Gets the function address (function pointer) of one function in the library from its symbol name. 

