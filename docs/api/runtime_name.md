# Name strings
## Classes
* [Luna::Name](class_luna_1_1_name.md)
## Alias types
* [using name_id_t =  u32](group___runtime_name_1ga025e1affb824b441b7da6b1ad7bb14ca.md)

    The name ID type. 

## Functions
* [const c8 * intern_name(const c8 *name)](group___runtime_name_1gaf329effc2cb74e7437566596886907f1.md)

    Interns one name string to the runtime and fetches the interned address for it. 

* [const c8 * intern_name(const c8 *name, usize count)](group___runtime_name_1ga370a2fa1c365f52c1b32960866efbe1e.md)

    Interns one name string to the runtime and fetches the interned address for it. 

* [void retain_name(const c8 *name)](group___runtime_name_1gad8142400d090a87429d19e8d149585f1.md)

    Increases the reference count of the name string by 1. 

* [void release_name(const c8 *name)](group___runtime_name_1ga752306e6c9de3a73e7eac1d2945880a0.md)

    Decreases the reference count of the name string by 1, and eventually frees the name string when the reference count goes to 0. 

* [name_id_t get_name_id(const c8 *name)](group___runtime_name_1ga13f8dd62c783ea811ceec70c99da153d.md)

    Gets the ID for the specified name. The ID keeps constant between multiple processes. 

* [usize get_name_size(const c8 *name)](group___runtime_name_1ga730737dfb3a218b8773cabd09e3c6f98.md)

    Fetches the size of the name string. 

* [typeinfo_t name_type()](group___runtime_name_1ga67c299d54605e7a80a6f4a2c3634bedf.md)

    Gets the type object of [Name](class_luna_1_1_name.md). 

