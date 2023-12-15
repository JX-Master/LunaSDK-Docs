# Name strings
## Classes
* [Luna::Name](class_luna_1_1_name.md)
## Aliasing types
* [using name_id_t =  u32](group___runtime_name_1ga025e1affb824b441b7da6b1ad7bb14ca.md)

    The name ID type. 

## Functions
* [LUNA_RUNTIME_API const c8 * intern_name(const c8 *name)](group___runtime_name_1gaa261ca6305ee4dee587492a004d6f9ee.md)

    Interns one name string to the runtime and fetches the interned address for it. 

* [LUNA_RUNTIME_API const c8 * intern_name(const c8 *name, usize count)](group___runtime_name_1ga8934afb8e4b840f7082726a1524428b9.md)

    Interns one name string to the runtime and fetches the interned address for it. 

* [LUNA_RUNTIME_API void retain_name(const c8 *name)](group___runtime_name_1ga7ad9785f8cb93e89864efc9507be5d0c.md)

    Increases the reference count of the name string by 1. 

* [LUNA_RUNTIME_API void release_name(const c8 *name)](group___runtime_name_1ga5556ed51beb79868d1c0f036ea3aa04d.md)

    Decreases the reference count of the name string by 1, and eventually frees the name string when the reference count goes to 0. 

* [LUNA_RUNTIME_API name_id_t get_name_id(const c8 *name)](group___runtime_name_1ga90645b965adcbec040490dcc08e617aa.md)

    Gets the ID for the specified name. The ID keeps constant between multiple processes. 

* [LUNA_RUNTIME_API usize get_name_size(const c8 *name)](group___runtime_name_1ga139e86dc82b131fa81bc73a33087cab8.md)

    Fetches the size of the name string. 

* [LUNA_RUNTIME_API typeinfo_t name_type()](group___runtime_name_1gafbf11b1c0e70c85b09db99aa4f786933.md)

    Gets the type object of [Name](class_luna_1_1_name.md). 

