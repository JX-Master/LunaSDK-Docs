# Boxed objects
## Alias types
* [using object_t =  opaque_t](group___runtime_object_1ga4d287a1c3bd0821c2391f4613686e35a.md)

    The opaque pointer that points to the boxed object. 

* [using ref_count_t =  i32](group___runtime_object_1gaa7422c517659edae01f5701669e17b26.md)

    The reference counter type for boxed objects. 

## Functions
* [typeinfo_t register_boxed_type()](group___runtime_object_1ga316fa5c9dec593e4cab7782fd8e64463.md)

    Registers one type so that it can be used for creating boxed objects. 

* [object_t object_alloc(typeinfo_t type)](group___runtime_object_1gabbcaac45f20e9e4c322fb1db0376b641.md)

    Allocates one boxed object. 

* [ref_count_t object_retain(object_t object_ptr)](group___runtime_object_1ga58de8f9cd270cba319bf80ec78fe51a7.md)

    Increases the strong refernece counter value by one. 

* [ref_count_t object_release(object_t object_ptr)](group___runtime_object_1ga7f822bf9876967630b4090507fff9465.md)

    Decreases the strong refernece counter value by one, and destroys the object if the reference counter drops to 0. 

* [ref_count_t object_ref_count(object_t object_ptr)](group___runtime_object_1ga649ddc0df3cdb7de5b618e692c35422c.md)

    Fetches the strong refernece counter value of the boxed object. 

* [ref_count_t object_retain_weak(object_t object_ptr)](group___runtime_object_1gab248f4fee54777f33eca884e848e5c06.md)

    Increases the weak refernece counter value by one. 

* [ref_count_t object_release_weak(object_t object_ptr)](group___runtime_object_1ga7db877575d1b92c06f6f0c574b93d15a.md)

    Decreases the weak refernece counter value by one. 

* [ref_count_t object_weak_ref_count(object_t object_ptr)](group___runtime_object_1ga19abee83cfb28d61706d21b381ef19b6.md)

    Fetches the weak refernece counter value of the boxed object. 

* [bool object_expired(object_t object_ptr)](group___runtime_object_1ga50969679bdddcd28a4f928c1da2959a7.md)

    Checks if the boxed object is expired, that is, destructed but its memeory is not freed. 

* [bool object_retain_if_not_expired(object_t object_ptr)](group___runtime_object_1ga9b9cee2ec7070dbd1b08dce660286306.md)

    Increases the strong refernece counter value by one if the boxed object is not expired. 

* [typeinfo_t get_object_type(object_t object_ptr)](group___runtime_object_1gaaaf5d608c320cd98447d41b15d8978b0.md)

    Gets the type object of the boxed object. 

* [bool object_is_type(object_t object_ptr, typeinfo_t type)](group___runtime_object_1gaad33cfe88e42fcc1929b7949b6d8574f.md)

    Checks whether the boxed object is the specified type or derived types of the specified type. 

* [_Rty * cast_object(object_t object_ptr)](group___runtime_object_1ga9b42ae46efc0d90e598a95e04187e5d8.md)

    Casts the object to the specified type. 

