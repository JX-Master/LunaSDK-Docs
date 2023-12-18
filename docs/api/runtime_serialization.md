# Serialization
## Classes
* [Luna::SerializableTypeDesc](struct_luna_1_1_serializable_type_desc.md)
## Alias types
* [using serialize_func_t =  R<Variant>(typeinfo_t type, const void* inst)](group___runtime_serialization_1ga45c924a8136fdc66c3db539f9e0c0a41.md)

    The serialization function for one instance. 

* [using deserialize_func_t =  RV(typeinfo_t type, void* inst, const Variant& data)](group___runtime_serialization_1gaf4acf5fc13de8c001cb46c680cba589b.md)

    The deserialization function for one instance. 

## Functions
* [bool is_type_serializable(typeinfo_t type)](group___runtime_serialization_1ga68bc4c02766d6c46c170d5266897f551.md)

    Checks whether one type is serializable. 

* [void set_serializable(typeinfo_t type, SerializableTypeDesc *desc=nullptr)](group___runtime_serialization_1ga1f1684079655c909c53a7c3ffa916a5a.md)

    Sets one type to be serializable. 

* [void set_serializable(SerializableTypeDesc *desc=nullptr)](group___runtime_serialization_1ga47944dee94b7b65503b429b073bd8cb3.md)

    Sets one type `_Ty` to be serializable. 

* [R< Variant > serialize(typeinfo_t type, const void *inst)](group___runtime_serialization_1gadbc56f9e44fcbc205ef78a64a00e450d.md)

    Serializes one instance. 

* [R< Variant > serialize(const _Ty &inst)](group___runtime_serialization_1ga233e0d1b7a4c8c7d7fa8f6d2ae1d13a1.md)

    Serializes one instance of type `_Ty`. 

* [RV deserialize(typeinfo_t type, void *inst, const Variant &data)](group___runtime_serialization_1gae38e1193604336f0c9f7309046a4d014.md)

    Deserializes one value. 

* [RV deserialize(_Ty &inst, const Variant &data)](group___runtime_serialization_1ga2d6e026e3ce699ccb752d84755e9b90d.md)

    Deserializes one value of type `_Ty`. 

