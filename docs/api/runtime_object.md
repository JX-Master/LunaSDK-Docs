# Boxed objects
## Aliasing types
* [using object_t =  opaque_t](group___runtime_object_1ga4d287a1c3bd0821c2391f4613686e35a.md)

    The opaque pointer that points to the boxed object. 

* [using ref_count_t =  i32](group___runtime_object_1gaa7422c517659edae01f5701669e17b26.md)

    The reference counter type for boxed objects. 

## Functions
* [typeinfo_t register_boxed_type()](group___runtime_object_1ga316fa5c9dec593e4cab7782fd8e64463.md)

    Registers one type so that it can be used for creating boxed objects. 

* [LUNA_RUNTIME_API object_t object_alloc(typeinfo_t type)](group___runtime_object_1ga8ba411b5dc3e81b9d5c0283752e22b9e.md)

    Allocates one boxed object. 

* [LUNA_RUNTIME_API ref_count_t object_retain(object_t object_ptr)](group___runtime_object_1ga05292c794e05337d2f55793b8a543a3d.md)

    Increases the strong refernece counter value by one. 

* [LUNA_RUNTIME_API ref_count_t object_release(object_t object_ptr)](group___runtime_object_1ga841b0eea4b1450118695a1ea1e323e54.md)

    Decreases the strong refernece counter value by one, and destroys the object if the reference counter drops to 0. 

* [LUNA_RUNTIME_API ref_count_t object_ref_count(object_t object_ptr)](group___runtime_object_1gae913d9c4fe24b3ce1bde56cc32f11a26.md)

    Fetches the strong refernece counter value of the boxed object. 

* [LUNA_RUNTIME_API ref_count_t object_retain_weak(object_t object_ptr)](group___runtime_object_1ga16a414bc273f61c5b494bbfeede47dc8.md)

    Increases the weak refernece counter value by one. 

* [LUNA_RUNTIME_API ref_count_t object_release_weak(object_t object_ptr)](group___runtime_object_1ga68c6d4e3df6b4ac39a9963b13a438a3a.md)

    Decreases the weak refernece counter value by one. 

* [LUNA_RUNTIME_API ref_count_t object_weak_ref_count(object_t object_ptr)](group___runtime_object_1gab006a9ca608307374757bc7d9bdd8c20.md)

    Fetches the weak refernece counter value of the boxed object. 

* [LUNA_RUNTIME_API bool object_expired(object_t object_ptr)](group___runtime_object_1ga5f1ea1fdc9db2b3f2bc17d22acfda13f.md)

    Checks if the boxed object is expired, that is, destructed but its memeory is not freed. 

* [LUNA_RUNTIME_API bool object_retain_if_not_expired(object_t object_ptr)](group___runtime_object_1ga86ba8bb53caec919089287e4b89aa0b0.md)

    Increases the strong refernece counter value by one if the boxed object is not expired. 

* [LUNA_RUNTIME_API typeinfo_t get_object_type(object_t object_ptr)](group___runtime_object_1ga7693a4a4b103ca1bb0fa1e41ea795ce2.md)

    Gets the type object of the boxed object. 

* [LUNA_RUNTIME_API bool object_is_type(object_t object_ptr, typeinfo_t type)](group___runtime_object_1gabe23034b4be97972a3340bbc70165eb8.md)

    Checks whether the boxed object is the specified type or derived types of the specified type. 

* [_Rty * cast_object(object_t object_ptr)](group___runtime_object_1ga9b42ae46efc0d90e598a95e04187e5d8.md)

    Casts the object to the specified type. 

