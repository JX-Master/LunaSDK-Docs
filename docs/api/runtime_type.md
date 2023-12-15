# Type reflection
## Classes
* [Luna::StructurePropertyDesc](struct_luna_1_1_structure_property_desc.md)
* [Luna::EnumerationOptionDesc](struct_luna_1_1_enumeration_option_desc.md)
* [Luna::StructureTypeDesc](struct_luna_1_1_structure_type_desc.md)
* [Luna::GenericStructureInstantiateInfo](struct_luna_1_1_generic_structure_instantiate_info.md)
* [Luna::GenericStructureTypeDesc](struct_luna_1_1_generic_structure_type_desc.md)
* [Luna::EnumerationTypeDesc](struct_luna_1_1_enumeration_type_desc.md)
* [Luna::typeof_t](struct_luna_1_1typeof__t.md)
## Aliasing types
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
* [LUNA_RUNTIME_API bool is_primitive_type(typeinfo_t type)](group___runtime_type_1gacb925e99451f18cdc4755041484bc58f.md)

    Checks whether one type is a primitive type. 

* [LUNA_RUNTIME_API bool is_struct_type(typeinfo_t type)](group___runtime_type_1gab8ed39307af0f42f486aa05ed104c4fb.md)

    Checks whether one type is a structure type. 

* [LUNA_RUNTIME_API bool is_enum_type(typeinfo_t type)](group___runtime_type_1ga075204ab589bdd65c9b1e8e47e76f083.md)

    Checks whether one type is an enumeration type. 

* [LUNA_RUNTIME_API bool is_generic_struct_type(typeinfo_t type)](group___runtime_type_1gadbb171090cd4af279f2dace82cd28978.md)

    Checks whether one type is a generic structure type. 

* [LUNA_RUNTIME_API bool is_generic_struct_instanced_type(typeinfo_t type)](group___runtime_type_1ga96250fce1e1c1c525229305336cf53f8.md)

    Checks whether one type is a generic instanced structure type. 

* [LUNA_RUNTIME_API typeinfo_t get_type_by_name(const Name &name, const Name &alias=Name())](group___runtime_type_1gac4c7a83d083ad87e8fcd53be7aa06b3b.md)

    Gets one type by its name. 

* [LUNA_RUNTIME_API Name get_type_name(typeinfo_t type, Name *alias=nullptr)](group___runtime_type_1ga421a9b78990b1995d7444af3ef0d4101.md)

    Gets the name of the specified type. 

* [LUNA_RUNTIME_API Guid get_type_guid(typeinfo_t type)](group___runtime_type_1ga53f50da16c89f016e6cb55776e898de5.md)

    Gets the GUID of the specified type. 

* [LUNA_RUNTIME_API usize get_type_size(typeinfo_t type)](group___runtime_type_1ga256cca8cf9ddc308d88ca53577c400f6.md)

    Gets the size of the specified type. 

* [LUNA_RUNTIME_API usize get_type_alignment(typeinfo_t type)](group___runtime_type_1ga28f229f2a3b27cce947cc16b3ad503d5.md)

    Gets the alignment requirement of the specified type. 

* [LUNA_RUNTIME_API void * get_type_private_data(typeinfo_t type, const Guid &data_guid)](group___runtime_type_1ga8b1f041ba85ca0a99ed545f814988f0a.md)

    Gets user defined private data for the specified type. 

* [LUNA_RUNTIME_API void * set_type_private_data(typeinfo_t type, const Guid &data_guid, usize data_size, usize data_alignment=0, void(*data_dtor)(void *)=nullptr)](group___runtime_type_1ga8eef2bb85d162fa168724baccc5950b2.md)

    Sets user defined private data for the specified type. 

* [LUNA_RUNTIME_API bool is_type_trivially_constructable(typeinfo_t type)](group___runtime_type_1ga7c158aa5c1cce13d8180b8042e2012d1.md)

    Checks whether one type is a trivially constructable type. 

* [LUNA_RUNTIME_API bool is_type_trivially_destructable(typeinfo_t type)](group___runtime_type_1ga31dcafde1f1f260367f617b28bd5221d.md)

    Checks whether one type is a trivially destructable type. 

* [LUNA_RUNTIME_API bool is_type_trivially_copy_constructable(typeinfo_t type)](group___runtime_type_1ga2291b986578001ab1974906279718f79.md)

    Checks whether one type is a trivially copy constructable type. 

* [LUNA_RUNTIME_API bool is_type_trivially_move_constructable(typeinfo_t type)](group___runtime_type_1ga601f7a22febe9a72e0f719a62db734e3.md)

    Checks whether one type is a trivially move constructable type. 

* [LUNA_RUNTIME_API bool is_type_trivially_copy_assignable(typeinfo_t type)](group___runtime_type_1gaa3ff6510d8913db109a24fe7b584821e.md)

    Checks whether one type is a trivially copy assignable type. 

* [LUNA_RUNTIME_API bool is_type_trivially_move_assignable(typeinfo_t type)](group___runtime_type_1gab8c3f4867cb9674acad87d4eb69ddd9b.md)

    Checks whether one type is a trivially move assignable type. 

* [LUNA_RUNTIME_API bool is_type_trivially_relocatable(typeinfo_t type)](group___runtime_type_1gaafacc048375e4353604b39ce2a114390.md)

    Checks whether one type is a trivially relocatable type. 

* [LUNA_RUNTIME_API void construct_type(typeinfo_t type, void *data)](group___runtime_type_1ga6a69b76cea1f8092be19f8a2205465d1.md)

    Constructs one instance of the specified type. 

* [LUNA_RUNTIME_API void construct_type_range(typeinfo_t type, void *data, usize count)](group___runtime_type_1gab59255ba7d0106421370d19ceb2c9132.md)

    Constructs one array of instances of the specified type. 

* [LUNA_RUNTIME_API void destruct_type(typeinfo_t type, void *data)](group___runtime_type_1ga89512f37edb473f255611970ac49d7d4.md)

    Destructs one instance of the specified type. 

* [LUNA_RUNTIME_API void destruct_type_range(typeinfo_t type, void *data, usize count)](group___runtime_type_1gaf2aa1b4875899673e912f966ba7ae33d.md)

    Destructs one array of instances of the specified type. 

* [LUNA_RUNTIME_API void copy_construct_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1ga5721a87baeb22e940c68ecbce2132278.md)

    Copy constructs one instance of the specified type. 

* [LUNA_RUNTIME_API void copy_construct_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1gac70c6be78b5040fd413a1d5401608f0c.md)

    Copy constructs one array of instances of the specified type. 

* [LUNA_RUNTIME_API void move_construct_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1gaedb52c18aad27367293256207fa535f0.md)

    Move constructs one instance of the specified type. 

* [LUNA_RUNTIME_API void move_construct_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1ga3c04bc45c180b05227a377a99517a1b4.md)

    Move constructs one array of instances of the specified type. 

* [LUNA_RUNTIME_API void copy_assign_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1gaba8a582259d93bbe88797de0adc53096.md)

    Copy assigns one instance of the specified type. 

* [LUNA_RUNTIME_API void copy_assign_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1ga6d917da49e3e129c8aa54e756969d145.md)

    Copy assigns one array of instances of the specified type. 

* [LUNA_RUNTIME_API void move_assign_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1gace6238035e555ee85eb9d8c046541209.md)

    Move assigns one instance of the specified type. 

* [LUNA_RUNTIME_API void move_assign_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1ga3bb128d9c6929bd3c112ccf5b4677eb4.md)

    Move assigns one array of instances of the specified type. 

* [LUNA_RUNTIME_API void relocate_type(typeinfo_t type, void *dst, void *src)](group___runtime_type_1ga6f2fd705b78706afba74ee787a7d4f90.md)

    Relocates one instance of the specified type. 

* [LUNA_RUNTIME_API void relocate_type_range(typeinfo_t type, void *dst, void *src, usize count)](group___runtime_type_1ga4990fdcdd72f56377d386e7b4a126e2b.md)

    Relocates one array of instances of the specified type. 

* [LUNA_RUNTIME_API bool is_type_equatable(typeinfo_t type)](group___runtime_type_1ga62226fa66d8019e672ad85dc4ba0af56.md)

    Checks whether the specified type supports equality testing. 

* [LUNA_RUNTIME_API void set_equatable(typeinfo_t type, equal_to_func_t *func)](group___runtime_type_1ga60e7625667f4239110c5f637d439de22.md)

    Sets one type to support equality testing. 

* [LUNA_RUNTIME_API bool equal_to_type(typeinfo_t type, const void *lhs, const void *rhs)](group___runtime_type_1ga10bd67f89151dedb1233dc37b32a5f66.md)

    Checks whether two instances of one type are equal. 

* [LUNA_RUNTIME_API bool is_type_hashable(typeinfo_t type)](group___runtime_type_1ga78831c040d8a8c9ab74622826ff16987.md)

    Checks whether the specified type supports hash code computing. 

* [LUNA_RUNTIME_API void set_hashable(typeinfo_t type, hash_func_t *func)](group___runtime_type_1gaae3393f0bc6ecd65157c1071c0363fc5.md)

    Sets one type to support hash code computing. 

* [LUNA_RUNTIME_API usize hash_type(typeinfo_t type, const void *inst)](group___runtime_type_1ga449f9f7a0ee098e3d913b13d4bb982b9.md)

    Computes the hash code of one instance of the specified type. 

* [LUNA_RUNTIME_API void set_type_attribute(typeinfo_t type, const Name &name, const Variant &value=Variant())](group___runtime_type_1ga9187115510c764871db92f2277882337.md)

    Sets one attribute of the specified type. 

* [LUNA_RUNTIME_API void remove_type_attribute(typeinfo_t type, const Name &name)](group___runtime_type_1ga8278384e54d76a31006942100c3e7842.md)

    Removes one attribute of the specified type. 

* [LUNA_RUNTIME_API bool check_type_attribute(typeinfo_t type, const Name &name)](group___runtime_type_1ga1e396c156aebdad0b1781db91cf3b81a.md)

    Checks whether the attribute of the specified type exists. 

* [LUNA_RUNTIME_API Variant get_type_attribute(typeinfo_t type, const Name &name)](group___runtime_type_1ga93cf43c9254f6baddc7052eefa0b566b.md)

    Gets the attribute of the specified type. 

* [LUNA_RUNTIME_API Vector< Name > get_type_attributes(typeinfo_t type)](group___runtime_type_1ga28e99ca7018d62261c58f4f8fa83102a.md)

    Gets all attributes of the specified type. 

* [LUNA_RUNTIME_API void set_property_attribute(typeinfo_t type, const Name &property, const Name &name, const Variant &value=Variant())](group___runtime_type_1gaba5ba232325b69268d9338520b941588.md)

    Sets one attribute of the specified property. 

* [LUNA_RUNTIME_API void remove_property_attribute(typeinfo_t type, const Name &property, const Name &name)](group___runtime_type_1gaa419dcaa7089913911cfb31cee11d59c.md)

    Removes one attribute of the specified property. 

* [LUNA_RUNTIME_API bool check_property_attribute(typeinfo_t type, const Name &property, const Name &name)](group___runtime_type_1ga7fc0735f26fc99cb3939654c5062f5bf.md)

    Checks whether the attribute of the specified property exists. 

* [LUNA_RUNTIME_API Variant get_property_attribute(typeinfo_t type, const Name &property, const Name &name)](group___runtime_type_1gadc1da372b065ba9a1527bb41efada5ab.md)

    Gets the attribute of the specified property. 

* [LUNA_RUNTIME_API Vector< Name > get_property_attributes(typeinfo_t type, const Name &property)](group___runtime_type_1gaaf4e28efc7b6a91e436bdefa98ff2f5b.md)

    Gets all attributes of the specified property. 

* [LUNA_RUNTIME_API typeinfo_t register_struct_type(const StructureTypeDesc &desc)](group___runtime_type_1ga949f118650021d610e817a18b0066f1e.md)

    Registers one structure type. 

* [LUNA_RUNTIME_API typeinfo_t register_generic_struct_type(const GenericStructureTypeDesc &desc)](group___runtime_type_1gacae380004370aab716f828f6a1aab8b2.md)

    Registers one generic structure type. 

* [LUNA_RUNTIME_API typeinfo_t register_enum_type(const EnumerationTypeDesc &desc)](group___runtime_type_1ga24af7db55ebbcf0f04b6a7052efb6e97.md)

    Registers one enumeration type. 

* [LUNA_RUNTIME_API Span< const StructurePropertyDesc > get_struct_properties(typeinfo_t type)](group___runtime_type_1gaf9d725af0b56a9ced503460f4d3fcc5d.md)

    Gets properties of the specified structure. 

* [LUNA_RUNTIME_API typeinfo_t get_base_type(typeinfo_t type)](group___runtime_type_1gabba17bf49390f1000f392d85bee0c0e4.md)

    Gets the base type of the specified type. 

* [LUNA_RUNTIME_API Span< const EnumerationOptionDesc > get_enum_options(typeinfo_t type)](group___runtime_type_1gafabfa3fe8f78913a9c3e59c3345718cd.md)

    Gets options of the specified enumeration. 

* [LUNA_RUNTIME_API typeinfo_t get_enum_underlying_type(typeinfo_t type)](group___runtime_type_1ga66233335688fb3b011425703194e25a0.md)

    Gets the underlying type of the specified enumeration. 

* [LUNA_RUNTIME_API bool is_multienum_type(typeinfo_t type)](group___runtime_type_1gacd2a1c1fbbbbfb12380928e96a243cc6.md)

    Checks if the specified type is a multi-value enumeration type. 

* [LUNA_RUNTIME_API i64 get_enum_instance_value(typeinfo_t type, const void *data)](group___runtime_type_1gaaeb4e0b057ba3b169bf1abcb22b3afe1.md)

    Extracts the mapped value of the enumeration, regardless of the underlying type of the enumeration. 

* [LUNA_RUNTIME_API void set_enum_instance_value(typeinfo_t type, void *data, i64 value)](group___runtime_type_1ga7a2013219b4087802ed59f166b4817d8.md)

    Sets the enumeration value to the specified mapped value. 

* [LUNA_RUNTIME_API typeinfo_t get_struct_generic_type(typeinfo_t type)](group___runtime_type_1gadb4a3944d98aeeb7e4880545a4eadd62.md)

    Gets the generic structure type from one generic structure instanced type. 

* [LUNA_RUNTIME_API Span< const typeinfo_t > get_struct_generic_arguments(typeinfo_t type)](group___runtime_type_1ga1233abc31d9f29e0a34815768863c867.md)

    Gets the generic arguments used to instantiate one generic structure instanced type. 

* [LUNA_RUNTIME_API Span< const Name > get_struct_generic_parameter_names(typeinfo_t type)](group___runtime_type_1ga3470c125e48b7e0aeeb4f7896cb1e000.md)

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

    Registers one structure type to the type system. The structure type must have one lustruct macro defined in the structure body. 

* [typeinfo_t register_enum_type(Span< const EnumerationOptionDesc > options, bool multienum=false)](group___runtime_type_1ga6c48e43cb9e673c260952a2ecedcec68.md)

    Registers one enumeration type to the type system. The enumeration type must have one luenum macro defined directly in `Luna` namespace. 

* [LUNA_RUNTIME_API typeinfo_t get_type_by_guid(const Guid &guid)](group___runtime_type_1ga10cefa8483a22b6c92284e28b4eb14fa.md)

    Gets the type object from one type GUID. 

* [typeinfo_t typeof()](group___runtime_type_1ga13a36b97bddb354ee6046139b9d92f32.md)

    Gets the type object of the specified type. 

* [LUNA_RUNTIME_API typeinfo_t void_type()](group___runtime_type_1ga5fe6cc28e7279ede8cd8a12fd4925946.md)

    Gets the type object of `void` type. 

* [LUNA_RUNTIME_API typeinfo_t u8_type()](group___runtime_type_1ga90857089e684fcde426c43234d75eba4.md)

    Gets the type object of `u8` type. 

* [LUNA_RUNTIME_API typeinfo_t i8_type()](group___runtime_type_1gaf74e0adfe66962ba2d88c715ce6d6e4f.md)

    Gets the type object of `i8` type. 

* [LUNA_RUNTIME_API typeinfo_t u16_type()](group___runtime_type_1ga5701d323cc28da06fd13293a73d9e56d.md)

    Gets the type object of `u16` type. 

* [LUNA_RUNTIME_API typeinfo_t i16_type()](group___runtime_type_1gab7ce802a4f7f33f2abf66bdc24042031.md)

    Gets the type object of `i16` type. 

* [LUNA_RUNTIME_API typeinfo_t u32_type()](group___runtime_type_1ga53307266b96df44991adce722416b13b.md)

    Gets the type object of `u32` type. 

* [LUNA_RUNTIME_API typeinfo_t i32_type()](group___runtime_type_1ga0fb5c36a4a8544d9bc1cf5f66af6d36e.md)

    Gets the type object of `i32` type. 

* [LUNA_RUNTIME_API typeinfo_t u64_type()](group___runtime_type_1ga4374647f277ac89886417a4f547fde87.md)

    Gets the type object of `u64` type. 

* [LUNA_RUNTIME_API typeinfo_t i64_type()](group___runtime_type_1ga473fe0c9cb061c008707fb35992e00c6.md)

    Gets the type object of `i64` type. 

* [LUNA_RUNTIME_API typeinfo_t usize_type()](group___runtime_type_1ga07d873387008577c8e5a372b40d96ae8.md)

    Gets the type object of `usize` type. 

* [LUNA_RUNTIME_API typeinfo_t isize_type()](group___runtime_type_1ga8fc8a7fac5d7599464ea5e3084a0475e.md)

    Gets the type object of `isize` type. 

* [LUNA_RUNTIME_API typeinfo_t f32_type()](group___runtime_type_1ga1d4937912d2740c1e3ff9f1e1a8a92b1.md)

    Gets the type object of `f32` type. 

* [LUNA_RUNTIME_API typeinfo_t f64_type()](group___runtime_type_1gaee80e769dd7fa525e7947ff532f4b88b.md)

    Gets the type object of `f64` type. 

* [LUNA_RUNTIME_API typeinfo_t c8_type()](group___runtime_type_1ga60f4ae65d88e08c4e2e5b6d72dff97d5.md)

    Gets the type object of `c8` type. 

* [LUNA_RUNTIME_API typeinfo_t c16_type()](group___runtime_type_1gae1c35ba7724a2de8c23e85b744bdf955.md)

    Gets the type object of `c16` type. 

* [LUNA_RUNTIME_API typeinfo_t c32_type()](group___runtime_type_1ga450f57469632c799c022ac46a3050ffc.md)

    Gets the type object of `c32` type. 

* [LUNA_RUNTIME_API typeinfo_t boolean_type()](group___runtime_type_1ga081417a084d865b5b3195ce53fb1ca71.md)

    Gets the type object of `bool` type. 

* [LUNA_RUNTIME_API typeinfo_t guid_type()](group___runtime_type_1ga94511b2e9b30763064ccb2de035e9f37.md)

    Gets the type object of `[Guid](struct_luna_1_1_guid.md)` type. 

* [LUNA_RUNTIME_API typeinfo_t version_type()](group___runtime_type_1ga2462e671631244c9db0536b5305d0d45.md)

    Gets the type object of `Version` type. 

* [LUNA_RUNTIME_API typeinfo_t pair_type()](group___runtime_type_1ga61541a6cfa370e9428ef8a7c44a37654.md)

    Gets the type object of `[Pair](struct_luna_1_1_pair.md)` generic type. 

* [LUNA_RUNTIME_API typeinfo_t get_generic_instanced_type(typeinfo_t generic_type, Span< const typeinfo_t > generic_arguments)](group___runtime_type_1ga24a09db5f8cad2409ba7de8a2822dc93.md)

    Gets one instanced type of one generic type. 

