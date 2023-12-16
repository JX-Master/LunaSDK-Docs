# Luna::GenericStructureInstantiateInfo
Describes the information of one generic structure instantiation operation. 

```c++
struct Luna::GenericStructureInstantiateInfo
```

This is returned by the instantiation callback function when one new generic structure instanced type is required. 

## Member objects
* [usize size](struct_luna_1_1_generic_structure_instantiate_info_1a59f6400efda18d25d7b3cf3c2e7a3d3d.md)

    The size of the structure type, this should include the size for the base type of this type. 

* [usize alignment](struct_luna_1_1_generic_structure_instantiate_info_1a84c18f6f6874b7f530f0c3ffe156e3fb.md)

    The alignment of the structure type. 

* [typeinfo_t base_type](struct_luna_1_1_generic_structure_instantiate_info_1a04e4a2d458c31f2a64e8669d8568ead9.md)

    The base type of this structure type. 

* [structure_ctor_t* ctor](struct_luna_1_1_generic_structure_instantiate_info_1a8b562d2692e5808232b9a65c240e6103.md)
* [structure_dtor_t* dtor](struct_luna_1_1_generic_structure_instantiate_info_1aa498db50ab9c3d7f9f84c97b8c24ac63.md)

    The destructor function for this type. If `nullptr`, the default destructor will be used. 

* [structure_copy_ctor_t* copy_ctor](struct_luna_1_1_generic_structure_instantiate_info_1abf45ac6225b448e989e041b420830949.md)
* [structure_move_ctor_t* move_ctor](struct_luna_1_1_generic_structure_instantiate_info_1a66e83256edf26122efc9735284bf5573.md)

    The move constructor for this type. If `nullptr`, the default move constructor will be used. 

* [structure_copy_assign_t* copy_assign](struct_luna_1_1_generic_structure_instantiate_info_1a7daacf4ed7ed76c8c18eb17f3ff4b1ed.md)

    The copy assignment operator for this type. If `nullptr`, the default copy assignment operator will be used. 

* [structure_move_assign_t* move_assign](struct_luna_1_1_generic_structure_instantiate_info_1a49a2c551255183998b610cfabb0bc464.md)

    The mvoe assignment operator for this type. If `nullptr`, the default move assignment operator will be used. 

* [Array<StructurePropertyDesc> properties](struct_luna_1_1_generic_structure_instantiate_info_1a9d4b7ec2acd9a6841c13e7ebd0262f23.md)

    The properties of this structure type. 

* [bool trivially_relocatable](struct_luna_1_1_generic_structure_instantiate_info_1a8e5f4fefafed4000ee467f8de565955d.md)

    Whether this structure is trivially relocatable. 

