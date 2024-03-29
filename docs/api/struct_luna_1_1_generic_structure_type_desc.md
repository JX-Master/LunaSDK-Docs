# Luna::GenericStructureTypeDesc
Describes one generic structure type. 

```c++
struct Luna::GenericStructureTypeDesc
```

## Member objects
* [Guid guid](struct_luna_1_1_generic_structure_type_desc_1a0c8f65c9d3118ff62b1d40950e5154f8.md)

    The GUID of the structure type. This should be unique for every type. 

* [Name name](struct_luna_1_1_generic_structure_type_desc_1a7082db574ba2d2d69ccafb060398b7d8.md)

    The name of the structure type. 

* [Name alias](struct_luna_1_1_generic_structure_type_desc_1aab3519e6b2915ade2b650f777b994121.md)

    The alias of the structure type. This can be empty. The alias is used to identify types with the same name. This can be used for generic specialization types. 

* [Span<const Name> generic_parameter_names](struct_luna_1_1_generic_structure_type_desc_1a4fe38c70c80a420b798584bc3c75063c.md)

    The names for every generic parameter. This is only used as hints for users. 

* [bool variable_generic_parameters](struct_luna_1_1_generic_structure_type_desc_1af6d3f22f30f3fda40c0f41afa1058614.md)

    Whether this type suports variable number of generic arguments. If this is `true`, the user may specify zero, one or more generic arguments after arguments specified in `generic_argument_names`. This is only used as hints for users. 

* [generic_structure_instantiate_t* instantiate](struct_luna_1_1_generic_structure_type_desc_1a5b11fda769284800e8a89d90d9873035.md)

    The function used to create generic instants for this generic type. 

