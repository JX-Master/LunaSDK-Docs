# Luna::StructureTypeDesc
Describes one structure type. 

```c++
struct Luna::StructureTypeDesc
```

## Member objects
* [Guid guid](struct_luna_1_1_structure_type_desc_1a0c8f65c9d3118ff62b1d40950e5154f8.md)

    The GUID of the structure type. This should be unique for every type. 

* [Name name](struct_luna_1_1_structure_type_desc_1a7082db574ba2d2d69ccafb060398b7d8.md)

    The name of the structure type. 

* [Name alias](struct_luna_1_1_structure_type_desc_1aab3519e6b2915ade2b650f777b994121.md)

    The alias of the structure type. This can be empty. The alias is used to identify types with the same name. This can be used for generic specialization types. 

* [usize size](struct_luna_1_1_structure_type_desc_1a59f6400efda18d25d7b3cf3c2e7a3d3d.md)

    The size of the structure type, this should include the size for the base type of this type. 

* [usize alignment](struct_luna_1_1_structure_type_desc_1a84c18f6f6874b7f530f0c3ffe156e3fb.md)

    The alignment of the structure type. 

* [typeinfo_t base_type](struct_luna_1_1_structure_type_desc_1a04e4a2d458c31f2a64e8669d8568ead9.md)

    The base type of this structure type. 

* [structure_ctor_t* ctor](struct_luna_1_1_structure_type_desc_1a8b562d2692e5808232b9a65c240e6103.md)

    The constructor function for this type. If `nullptr`, the default constructor will be used. See remarks of [construct_type](group___runtime_type_1ga90deafaf36d47cd50f7af0b53f30dac5.md) for default constructor behavior. 

* [structure_dtor_t* dtor](struct_luna_1_1_structure_type_desc_1aa498db50ab9c3d7f9f84c97b8c24ac63.md)

    The destructor function for this type. If `nullptr`, the default destructor will be used. See remarks of [destruct_type](group___runtime_type_1gaf8ad2e47bfbc89371f6d2ef227c39f28.md) for default constructor behavior. 

* [structure_copy_ctor_t* copy_ctor](struct_luna_1_1_structure_type_desc_1abf45ac6225b448e989e041b420830949.md)

    The copy constructor for this type. If `nullptr`, the default copy constructor will be used. See remarks of [copy_construct_type](group___runtime_type_1ga5f69494b37cb69b3547cdce14b5b1087.md) for default constructor behavior. 

* [structure_move_ctor_t* move_ctor](struct_luna_1_1_structure_type_desc_1a66e83256edf26122efc9735284bf5573.md)

    The move constructor for this type. If `nullptr`, the default move constructor will be used. See remarks of [move_construct_type](group___runtime_type_1gac7867a132f5246297db7b59105df8f9b.md) for default constructor behavior. 

* [structure_copy_assign_t* copy_assign](struct_luna_1_1_structure_type_desc_1a7daacf4ed7ed76c8c18eb17f3ff4b1ed.md)

    The copy assignment operator for this type. If `nullptr`, the default copy assignment operator will be used. See remarks of [copy_assign_type](group___runtime_type_1gadda24f3e17aeb6be651380445522e3e6.md) for default constructor behavior. 

* [structure_move_assign_t* move_assign](struct_luna_1_1_structure_type_desc_1a49a2c551255183998b610cfabb0bc464.md)

    The mvoe assignment operator for this type. If `nullptr`, the default move assignment operator will be used. See remarks of [move_assign_type](group___runtime_type_1gade978350a36e3988fc4c6a5894a96465.md) for default constructor behavior. 

* [Span<const StructurePropertyDesc> properties](struct_luna_1_1_structure_type_desc_1a9b43bf1a828e7baefd0522a2563c66f2.md)

    The properties of this structure type. 

* [bool trivially_relocatable](struct_luna_1_1_structure_type_desc_1a8e5f4fefafed4000ee467f8de565955d.md)

    Whether this structure is trivially relocatable. One structure is trivially relocatable if its content can be moved to another memory address using memcpy, and using the instance on new memory location behaves the same as the instance on old memory location. 

