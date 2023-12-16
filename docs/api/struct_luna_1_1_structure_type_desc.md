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
* [usize size](struct_luna_1_1_structure_type_desc_1a59f6400efda18d25d7b3cf3c2e7a3d3d.md)

    The size of the structure type, this should include the size for the base type of this type. 

* [usize alignment](struct_luna_1_1_structure_type_desc_1a84c18f6f6874b7f530f0c3ffe156e3fb.md)

    The alignment of the structure type. 

* [typeinfo_t base_type](struct_luna_1_1_structure_type_desc_1a04e4a2d458c31f2a64e8669d8568ead9.md)

    The base type of this structure type. 

* [structure_ctor_t* ctor](struct_luna_1_1_structure_type_desc_1a8b562d2692e5808232b9a65c240e6103.md)
* [structure_dtor_t* dtor](struct_luna_1_1_structure_type_desc_1aa498db50ab9c3d7f9f84c97b8c24ac63.md)
* [structure_copy_ctor_t* copy_ctor](struct_luna_1_1_structure_type_desc_1abf45ac6225b448e989e041b420830949.md)
* [structure_move_ctor_t* move_ctor](struct_luna_1_1_structure_type_desc_1a66e83256edf26122efc9735284bf5573.md)
* [structure_copy_assign_t* copy_assign](struct_luna_1_1_structure_type_desc_1a7daacf4ed7ed76c8c18eb17f3ff4b1ed.md)
* [structure_move_assign_t* move_assign](struct_luna_1_1_structure_type_desc_1a49a2c551255183998b610cfabb0bc464.md)
* [Span<const StructurePropertyDesc> properties](struct_luna_1_1_structure_type_desc_1a9b43bf1a828e7baefd0522a2563c66f2.md)

    The properties of this structure type. 

* [bool trivially_relocatable](struct_luna_1_1_structure_type_desc_1a8e5f4fefafed4000ee467f8de565955d.md)
