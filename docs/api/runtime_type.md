# Type reflection
## Types
* [Luna::StructurePropertyDesc](struct_luna_1_1_structure_property_desc.md)

    Describes one structure property. 


* [Luna::EnumerationOptionDesc](struct_luna_1_1_enumeration_option_desc.md)

    Describes one enumeration option. 


* [Luna::StructureTypeDesc](struct_luna_1_1_structure_type_desc.md)

    Describes one structure type. 


* [Luna::GenericStructureInstantiateInfo](struct_luna_1_1_generic_structure_instantiate_info.md)

    Describes the information of one generic structure instantiation operation. 


* [Luna::GenericStructureTypeDesc](struct_luna_1_1_generic_structure_type_desc.md)

    Describes one generic structure type. 


* [Luna::EnumerationTypeDesc](struct_luna_1_1_enumeration_type_desc.md)

    Describes one enumeration type. 


* [Luna::typeof_t](struct_luna_1_1typeof__t.md)

    The functional obejct that can be overloaded to define custom behavior of [typeof](group___runtime_type_1ga13a36b97bddb354ee6046139b9d92f32.md) for user-defined types. 


## Alias types
* [using equal_to_func_t =  bool(typeinfo_t type, const void* lhs, const void* rhs)](group___runtime_type_1gaa25ce33574555d8be053cd84f12d64a6.md)

    The equality testing function used by the reflection system. 

* [using hash_func_t =  usize(typeinfo_t type, const void* inst)](group___runtime_type_1ga909db1d9ee83e74969fc1fa2886e5e6e.md)

    The hash code computing function used by the reflection system. 

* [using structure_ctor_t =  void(typeinfo_t type, void* inst)](group___runtime_type_1ga768ca9e582a3c0b845ace5631983cd71.md)

    The structure constructor used by the reflection system. 

* [using structure_dtor_t =  void(typeinfo_t type, void* inst)](group___runtime_type_1gaeee4991fbe3240a564266b083ae20350.md)

    The structure destructor used by the reflection system. 

* [using structure_copy_ctor_t =  void(typeinfo_t type, void* dst, void* src)](group___runtime_type_1ga95dd21bb12c6ba99ba17a4199b250861.md)

    The structure copy constructor used by the reflection system. 

* [using structure_move_ctor_t =  void(typeinfo_t type, void* dst, void* src)](group___runtime_type_1ga30fdab15e426d873fca3b5c56582ac01.md)

    The structure move constructor used by the reflection system. 

* [using structure_copy_assign_t =  void(typeinfo_t type, void* dst, void* src)](group___runtime_type_1ga7e173d3716124b458d3cab6b996b1d33.md)

    The structure copy assignment operator used by the reflection system. 

* [using structure_move_assign_t =  void(typeinfo_t type, void* dst, void* src)](group___runtime_type_1gaf8b43f55564bdc0df9aa4e2ff26e0166.md)

    The structure move assignment operator used by the reflection system. 

* [using generic_structure_instantiate_t =  GenericStructureInstantiateInfo(typeinfo_t generic_type, Span<const typeinfo_t> generic_arguments)](group___runtime_type_1ga2fed0c2819a727130c18322aef9e8381.md)

    The generic structure instantiation function called by the reflection system when one new generic structure instanced type is required. 

* [using typeinfo_t =  opaque_t](group___runtime_type_1ga100c23d7c000bc0c5f14d87f172425f2.md)

    The opaque pointer that points to one type object. 

## Functions
* [bool is_primitive_type(typeinfo_t type)](group___runtime_type_1gae7f576c36829b6b9b8ad6c710d657721.md)

    Checks whether one type is a primitive type. 

* [bool is_struct_type(typeinfo_t type)](group___runtime_type_1ga1b61643f0a4bcf6acf3204bd11b32571.md)

    Checks whether one type is a structure type. 

* [bool is_enum_type(typeinfo_t type)](group___runtime_type_1gad65f8ca0ae6c3ad6d8209183ca9ed7f5.md)

    Checks whether one type is an enumeration type. 

* [bool is_generic_struct_type(typeinfo_t type)](group___runtime_type_1gafdfdfc8bba93ff6674813a7423f91adb.md)

    Checks whether one type is a generic structure type. 

* [bool is_generic_struct_instanced_type(typeinfo_t type)](group___runtime_type_1gad679df80c8814f176167d5e76dabf709.md)

    Checks whether one type is a generic instanced structure type. 

* [typeinfo_t get_type_by_name(const Name &name, const Name &alias=Name())](group___runtime_type_1ga6453dd75e7fc9b8bd6bbcb2d11e91a23.md)

    Gets one type by its name. 

* [Name get_type_name(typeinfo_t type, Name *alias=nullptr)](group___runtime_type_1ga52ac5a9e9ddf278731aa9ebf1ed517e6.md)

    Gets the name of the specified type. 

* [Guid get_type_guid(typeinfo_t type)](group___runtime_type_1ga7fda487a8b768f2bf68ef190c6cab11f.md)

    Gets the GUID of the specified type. 

* [usize get_type_size(typeinfo_t type)](group___runtime_type_1gad3d4b2f80d7b177bc07f84e1f8ef5d15.md)

    Gets the size of the specified type. 

* [usize get_type_alignment(typeinfo_t type)](group___runtime_type_1gac22dfcf97be70832ae7cf4693501e604.md)

    Gets the alignment requirement of the specified type. 

* [void * get_type_private_data(typeinfo_t type, const Guid &data_guid)](group___runtime_type_1ga9f4f6c0054fd660740373b5e43815b6a.md)

    Gets user defined private data for the specified type. 

* [void * set_type_private_data(typeinfo_t type, const Guid &data_guid, usize data_size, usize data_alignment=0, void(*data_dtor)(void *)=nullptr)](group___runtime_type_1ga93f22e760ffc9e4df3f168086c062405.md)

    Sets user defined private data for the specified type. 

* [bool is_type_trivially_constructable(typeinfo_t type)](group___runtime_type_1ga2fe52be7fd03cf44df337b027d79e11c.md)

    Checks whether one type is a trivially constructable type. 

* [bool is_type_trivially_destructable(typeinfo_t type)](group___runtime_type_1ga01686ee3f37d770b5122299fbc111f0f.md)

    Checks whether one type is a trivially destructable type. 

* [bool is_type_trivially_copy_constructable(typeinfo_t type)](group___runtime_type_1gaf70cfe2918cd27b4784b40856c3aebcc.md)

    Checks whether one type is a trivially copy constructable type. 

* [bool is_type_trivially_move_constructable(typeinfo_t type)](group___runtime_type_1ga5600e3653e871f80dfc6fd8755ec4c8c.md)

    Checks whether one type is a trivially move constructable type. 

* [bool is_type_trivially_copy_assignable(typeinfo_t type)](group___runtime_type_1ga03c69cf7de86f75bbf1af884984e6e8a.md)

    Checks whether one type is a trivially copy assignable type. 

* [bool is_type_trivially_move_assignable(typeinfo_t type)](group___runtime_type_1ga2926539da4b05ee50a8d2e80c996764a.md)

    Checks whether one type is a trivially move assignable type. 

* [bool is_type_trivially_relocatable(typeinfo_t type)](group___runtime_type_1gae0965bf3d0302675dab045d734ea18d2.md)

    Checks whether one type is a trivially relocatable type. 

* [void construct_type(typeinfo_t type, void *data)](group___runtime_type_1ga90deafaf36d47cd50f7af0b53f30dac5.md)

    Constructs one instance of the specified type. 

* [void construct_type_range(typeinfo_t type, void *data, usize count)](group___runtime_type_1ga16761cb0215c3514de9b926013baaa54.md)

    Constructs one array of instances of the specified type. 

* [void destruct_type(typeinfo_t type, void *data)](group___runtime_type_1gaf8ad2e47bfbc89371f6d2ef227c39f28.md)

    Destructs one instance of the specified type. 

* [void destruct_type_range(typeinfo_t type, void *data, usize count)](group___runtime_type_1ga29830e9e952d335ae7b29d209a71470d.md)

    Destructs one array of instances of the specified type. 

* [void copy_construct_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1ga5f69494b37cb69b3547cdce14b5b1087.md)

    Copy constructs one instance of the specified type. 

* [void copy_construct_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1ga76a4b4445cefe0a698e12b4439be3afc.md)

    Copy constructs one array of instances of the specified type. 

* [void move_construct_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1gac7867a132f5246297db7b59105df8f9b.md)

    Move constructs one instance of the specified type. 

* [void move_construct_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1gacd4e18bbaee9d1a85bfddf361ce423a5.md)

    Move constructs one array of instances of the specified type. 

* [void copy_assign_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1gadda24f3e17aeb6be651380445522e3e6.md)

    Copy assigns one instance of the specified type. 

* [void copy_assign_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1ga18af6c49a0c8efc9627fdce8064bfe61.md)

    Copy assigns one array of instances of the specified type. 

* [void move_assign_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1gade978350a36e3988fc4c6a5894a96465.md)

    Move assigns one instance of the specified type. 

* [void move_assign_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1gac2b3174ddee187d72c3998e78791515a.md)

    Move assigns one array of instances of the specified type. 

* [void relocate_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1gac930bb80f894f032a8336095c530633c.md)

    Relocates one instance of the specified type. 

* [void relocate_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1ga5a6f6544ce77cc19816d5054f9b02d38.md)

    Relocates one array of instances of the specified type. 

* [bool is_type_equatable(typeinfo_t type)](group___runtime_type_1gadd9581f23fe9b07267ce37d34223fdff.md)

    Checks whether the specified type supports equality testing. 

* [void set_equatable(typeinfo_t type, equal_to_func_t *func)](group___runtime_type_1ga855a64c6ebed3319fa105897418794cd.md)

    Sets one type to support equality testing. 

* [bool equal_to_type(typeinfo_t type, const void *lhs, const void *rhs)](group___runtime_type_1gaae983f2b7978277e6098795b0987e59c.md)

    Checks whether two instances of one type are equal. 

* [bool is_type_hashable(typeinfo_t type)](group___runtime_type_1ga504ecabdaf29473063881e06d3cf1190.md)

    Checks whether the specified type supports hash code computing. 

* [void set_hashable(typeinfo_t type, hash_func_t *func)](group___runtime_type_1ga47106eb319ea3bd9701505b03473b0a6.md)

    Sets one type to support hash code computing. 

* [usize hash_type(typeinfo_t type, const void *inst)](group___runtime_type_1ga9b8e281a809d26db7bb0e738b5de91ae.md)

    Computes the hash code of one instance of the specified type. 

* [void set_type_attribute(typeinfo_t type, const Name &name, const Variant &value=Variant())](group___runtime_type_1ga627b83ba0cf45ab0b13489dc1451149e.md)

    Sets one attribute of the specified type. 

* [void remove_type_attribute(typeinfo_t type, const Name &name)](group___runtime_type_1ga58b7940e0d0b2c59a886ca122d6ce710.md)

    Removes one attribute of the specified type. 

* [bool check_type_attribute(typeinfo_t type, const Name &name)](group___runtime_type_1gadea266de7221e6c8934e624a2c2406ef.md)

    Checks whether the attribute of the specified type exists. 

* [Variant get_type_attribute(typeinfo_t type, const Name &name)](group___runtime_type_1gae82fac9cfbc8d341bb965a69b95e961f.md)

    Gets the attribute of the specified type. 

* [Vector< Name > get_type_attributes(typeinfo_t type)](group___runtime_type_1ga4a69cabc206642ef6d643489e52f3be4.md)

    Gets all attributes of the specified type. 

* [void set_property_attribute(typeinfo_t type, const Name &property, const Name &name, const Variant &value=Variant())](group___runtime_type_1ga8e628ce8471510d154b1442ace10c78d.md)

    Sets one attribute of the specified property. 

* [void remove_property_attribute(typeinfo_t type, const Name &property, const Name &name)](group___runtime_type_1ga7d87d5eba14cc6d152a0afaae93bc866.md)

    Removes one attribute of the specified property. 

* [bool check_property_attribute(typeinfo_t type, const Name &property, const Name &name)](group___runtime_type_1ga35aa25238b78e2a5abe2eb1f68acb498.md)

    Checks whether the attribute of the specified property exists. 

* [Variant get_property_attribute(typeinfo_t type, const Name &property, const Name &name)](group___runtime_type_1gab18bd8bc8de3e0f55f570d95e50e86b8.md)

    Gets the attribute of the specified property. 

* [Vector< Name > get_property_attributes(typeinfo_t type, const Name &property)](group___runtime_type_1ga998734779bc45c1c7b72174addd44219.md)

    Gets all attributes of the specified property. 

* [typeinfo_t register_struct_type(const StructureTypeDesc &desc)](group___runtime_type_1gabdbbe8b5d92239b0af155d9d04b78f1c.md)

    Registers one structure type. 

* [typeinfo_t register_generic_struct_type(const GenericStructureTypeDesc &desc)](group___runtime_type_1gab1f730455f72135a6dfb8afedf212c23.md)

    Registers one generic structure type. 

* [typeinfo_t register_enum_type(const EnumerationTypeDesc &desc)](group___runtime_type_1ga23359d0927de35a14f18d2e4d86d17bb.md)

    Registers one enumeration type. 

* [Span< const StructurePropertyDesc > get_struct_properties(typeinfo_t type)](group___runtime_type_1gab0968ee0784979040f64e25a007a46d8.md)

    Gets properties of the specified structure. 

* [typeinfo_t get_base_type(typeinfo_t type)](group___runtime_type_1ga9397a27f3351369ed81815bc19b241c5.md)

    Gets the base type of the specified type. 

* [Span< const EnumerationOptionDesc > get_enum_options(typeinfo_t type)](group___runtime_type_1gaaf8822ea750a7f2d7aea628b293a9089.md)

    Gets options of the specified enumeration. 

* [typeinfo_t get_enum_underlying_type(typeinfo_t type)](group___runtime_type_1ga49b24123baef379224040581fa29f979.md)

    Gets the underlying type of the specified enumeration. 

* [bool is_multienum_type(typeinfo_t type)](group___runtime_type_1ga67682773704d1aa3f44a00325a853471.md)

    Checks if the specified type is a multi-value enumeration type. 

* [i64 get_enum_instance_value(typeinfo_t type, const void *data)](group___runtime_type_1ga09292900d650d5e6ad3b564ea87d9fe4.md)

    Extracts the mapped value of the enumeration, regardless of the underlying type of the enumeration. 

* [void set_enum_instance_value(typeinfo_t type, void *data, i64 value)](group___runtime_type_1ga50f2743d5d6b0469d6f5c821fa13d363.md)

    Sets the enumeration value to the specified mapped value. 

* [typeinfo_t get_struct_generic_type(typeinfo_t type)](group___runtime_type_1ga4fb0c09f015caf48f3ad4786d197592d.md)

    Gets the generic structure type from one generic structure instanced type. 

* [Span< const typeinfo_t > get_struct_generic_arguments(typeinfo_t type)](group___runtime_type_1gae55e06ac21d9b021aae1805078bd3a68.md)

    Gets the generic arguments used to instantiate one generic structure instanced type. 

* [Span< const Name > get_struct_generic_parameter_names(typeinfo_t type)](group___runtime_type_1ga63cb33b0f155e7cd55433c4e7454d1c0.md)

    Gets the generic parameter names of the specified type. 

* [bool default_equal_to(typeinfo_t type, const void *lhs, const void *rhs)](group___runtime_type_1gaba0b3d24063eba33f57dbfb077bb4531.md)

    The default equality comparison function used by the reflection system. 

* [usize default_hash(typeinfo_t type, const void *inst)](group___runtime_type_1ga618765ed95035e04b42690b1133a9f4b.md)

    The default hashing function used by the reflection system. 

* [void default_ctor(typeinfo_t type, void *inst)](group___runtime_type_1gacca2301b7b3699c1da3e644a26da55a8.md)

    The default constructor used by the reflection system. 

* [void default_dtor(typeinfo_t type, void *inst)](group___runtime_type_1ga90c85568f4936b27f83a9292e56e16fb.md)

    The default destructor used by the reflection system. 

* [void default_copy_ctor(typeinfo_t type, void *dst, void *src)](group___runtime_type_1gae3195fc4508a440ef12ebaca7895adcb.md)

    The default copy constructor used by the reflection system. 

* [void default_move_ctor(typeinfo_t type, void *dst, void *src)](group___runtime_type_1ga5aa5b57403b26df69146f732a663fe3b.md)

    The default move constructor used by the reflection system. 

* [void default_copy_assign(typeinfo_t type, void *dst, void *src)](group___runtime_type_1ga71c6c50c5adcab8d3f8640bad32ce061.md)

    The default copy assignment function used by the reflection system. 

* [void default_move_assign(typeinfo_t type, void *dst, void *src)](group___runtime_type_1ga101ae16d63173d8244de7d6d40f8341f.md)

    The default move assignment function used by the reflection system. 

* [typeinfo_t register_struct_type(Span< const StructurePropertyDesc > properties, typeinfo_t base_type=nullptr)](group___runtime_type_1gaef020b7b9d42e098afb57ed8676a863b.md)

    Registers one structure type to the type system. The structure type must have one [lustruct](group___runtime_type_1ga706ef093389171fcac4e2745b5a325a5.md) macro defined in the structure body. 

* [typeinfo_t register_enum_type(Span< const EnumerationOptionDesc > options, bool multienum=false)](group___runtime_type_1ga6c48e43cb9e673c260952a2ecedcec68.md)

    Registers one enumeration type to the type system. The enumeration type must have one [luenum](group___runtime_type_1gaa5c575c676819bd6348365fba48b6769.md) macro defined directly in `Luna` namespace. 

* [typeinfo_t get_type_by_guid(const Guid &guid)](group___runtime_type_1gae067905858c7ea088d2059362811ae57.md)

    Gets the type object from one type GUID. 

* [typeinfo_t typeof()](group___runtime_type_1ga13a36b97bddb354ee6046139b9d92f32.md)

    Gets the type object of the specified type. 

* [typeinfo_t void_type()](group___runtime_type_1ga26d2e49309c4cd37f58b4ca79f8b6361.md)

    Gets the type object of `void` type. 

* [typeinfo_t u8_type()](group___runtime_type_1ga032ad26036368d0d7ca738a13b33a2f2.md)

    Gets the type object of `u8` type. 

* [typeinfo_t i8_type()](group___runtime_type_1ga1e712a4cc4d17a63c3b1998284654e97.md)

    Gets the type object of `i8` type. 

* [typeinfo_t u16_type()](group___runtime_type_1ga226391463e5119e0a3c2d6da1c97aac7.md)

    Gets the type object of `u16` type. 

* [typeinfo_t i16_type()](group___runtime_type_1ga9ddf71ac213abc8f87dc45c2eb1fa10d.md)

    Gets the type object of `i16` type. 

* [typeinfo_t u32_type()](group___runtime_type_1gabee4d766699d26f20e3deb99708c475d.md)

    Gets the type object of `u32` type. 

* [typeinfo_t i32_type()](group___runtime_type_1ga762be3b0f0082f825607d4e46dadd0b4.md)

    Gets the type object of `i32` type. 

* [typeinfo_t u64_type()](group___runtime_type_1ga9a5d27367d755b8ace0aa84e76400167.md)

    Gets the type object of `u64` type. 

* [typeinfo_t i64_type()](group___runtime_type_1ga9422b3152edf32b6bdc67ce0e882a85a.md)

    Gets the type object of `i64` type. 

* [typeinfo_t usize_type()](group___runtime_type_1gad666e7c2bb1220f0b962488c2c64221d.md)

    Gets the type object of `usize` type. 

* [typeinfo_t isize_type()](group___runtime_type_1gabcc48c93609b10650858d655412199b9.md)

    Gets the type object of `isize` type. 

* [typeinfo_t f32_type()](group___runtime_type_1ga3053403f3538a058306b98d4a1bc85f9.md)

    Gets the type object of `f32` type. 

* [typeinfo_t f64_type()](group___runtime_type_1ga7a482800b36a03b26f53d2fd229ab26d.md)

    Gets the type object of `f64` type. 

* [typeinfo_t c8_type()](group___runtime_type_1gac35d7e909bb07c96dfd08c5d5829d6c3.md)

    Gets the type object of `c8` type. 

* [typeinfo_t c16_type()](group___runtime_type_1gac1d722a03cbbf86f6f5410e273d0d1c8.md)

    Gets the type object of `c16` type. 

* [typeinfo_t c32_type()](group___runtime_type_1ga27db53970eba5d91f761441938289542.md)

    Gets the type object of `c32` type. 

* [typeinfo_t boolean_type()](group___runtime_type_1gaca85d3f68ae05c414fd48c02cf76c64d.md)

    Gets the type object of `bool` type. 

* [typeinfo_t guid_type()](group___runtime_type_1ga3aa3ae2e7cce9bc3e663609a5600afa0.md)

    Gets the type object of `Guid` type. 

* [typeinfo_t version_type()](group___runtime_type_1ga27eeb1c9421cbf65c7fe64569588efb0.md)

    Gets the type object of `Version` type. 

* [typeinfo_t pair_type()](group___runtime_type_1ga118f6b8c5e5cd4755bc33987bda61ddb.md)

    Gets the type object of `Pair` generic type. 

* [typeinfo_t get_generic_instanced_type(typeinfo_t generic_type, Span< const typeinfo_t > generic_arguments)](group___runtime_type_1ga49059ae1daffad4476ce6c3f8ed127f7.md)

    Gets one instanced type of one generic type. 

## Macros
* [lustruct(_name, _guid)](group___runtime_type_1ga706ef093389171fcac4e2745b5a325a5.md)

    Declares the name and guid for one structure or class type. 

* [luproperty(_struct, _type, _name)](group___runtime_type_1gaa77d452893e669bfab5269edb321ff75.md)

    Declares one property used in [Luna::register_struct_type](group___runtime_type_1gabdbbe8b5d92239b0af155d9d04b78f1c.md). 

* [luenum(_type, _name, _guid)](group___runtime_type_1gaa5c575c676819bd6348365fba48b6769.md)

    Declares the name and guid for one enumeration type. 

* [luoption(_enum, _item)](group___runtime_type_1ga2c3ef7a6cd6e691e08c11d97650d53a5.md)

    Declares one option used in [Luna::register_enum_type](group___runtime_type_1ga23359d0927de35a14f18d2e4d86d17bb.md). 

