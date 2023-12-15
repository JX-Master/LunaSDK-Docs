# Runtime
Represents a waitable object used for multi-thread synchronization. 

The Runtime module provides the runtime environment of Luna SDK and defines core functionalities that will be used by almost all modules.

Objects that implements `IWaitable` cannot be used cross process boundary. 

## Topics
* [Algorithms](runtime_algorithm.md)
* [Containers](runtime_container.md)
* [Assertions](runtime_assert.md)
* [Atomic Operations](runtime_atomic.md)
* [Base64 encoding/decoding](runtime_base64.md)
* [Base85 encoding/decoding](runtime_base85.md)
* [Debugging](runtime_debug.md)
* [DLL loading](runtime_d_l_l.md)
* [Error handling](runtime_error.md)
* [Files](runtime_file.md)
* [Hashing functions](runtime_hash.md)
* [Interfaces](runtime_interface.md)
* [Logging](runtime_log.md)
* [Memory allocation and deallocation](runtime_memory.md)
* [Memory utility library](runtime_memory_utils.md)
* [Module system](runtime_module.md)
* [Name strings](runtime_name.md)
* [Boxed objects](runtime_object.md)
* [Path](runtime_path.md)
* [Debugging](runtime_profiler.md)
* [Generating random numbers](runtime_random.md)
* [SDK initialization and shutdown](runtime_init.md)
* [Thread management and synchronization methods](runtime_thread.md)
* [Type reflection](runtime_type.md)
* [Unicode encoding/decoding](runtime_unicode.md)
## Classes
* [Luna::Allocator](class_luna_1_1_allocator.md)
* [Luna::is_over_aligned](struct_luna_1_1is__over__aligned.md)
* [Luna::is_trivially_relocatable](struct_luna_1_1is__trivially__relocatable.md)
* [Luna::Guid](struct_luna_1_1_guid.md)
* [Luna::Pair](struct_luna_1_1_pair.md)
* [Luna::OptionalPair](class_luna_1_1_optional_pair.md)
* [Luna::Blob](class_luna_1_1_blob.md)
* [Luna::Event](class_luna_1_1_event.md)
* [Luna::equal_to](struct_luna_1_1equal__to.md)
* [Luna::less](struct_luna_1_1less.md)
* [Luna::hash](struct_luna_1_1hash.md)
* [Luna::ReferenceWrapper](class_luna_1_1_reference_wrapper.md)
* [Luna::Function< _R(_Args...)>](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4.md)
* [Luna::ReverseIterator](class_luna_1_1_reverse_iterator.md)
* [Luna::ObjRef](class_luna_1_1_obj_ref.md)
* [Luna::Ref](class_luna_1_1_ref.md)
* [Luna::WeakObjRef](class_luna_1_1_weak_obj_ref.md)
* [Luna::WeakRef](class_luna_1_1_weak_ref.md)
* [Luna::IStream](struct_luna_1_1_i_stream.md)
* [Luna::ISeekableStream](struct_luna_1_1_i_seekable_stream.md)
* [Luna::Variant](class_luna_1_1_variant.md)
* [Luna::Vector](class_luna_1_1_vector.md)
## Aliasing types
* [using u8 =  std::uint8_t](group___runtime_1ga254d32383658e016368673396e7afc1b.md)

    Unsigned 8-bit integer (0~255). 

* [using u16 =  std::uint16_t](group___runtime_1ga917e58b0692c2df778a27350534cbfe7.md)

    Unsigned 16-bit integer (0~65535). 

* [using u32 =  std::uint32_t](group___runtime_1ga65cf28726f89e62ccf2f1354bc2716df.md)

    Unsigned 32-bit integer (0~4294967295). 

* [using u64 =  std::uint64_t](group___runtime_1ga66e1d499241ccae9a18a20a1f4f0590d.md)

    Unsigned 64-bit integer (0~18446744073709551615). 

* [using i8 =  std::int8_t](group___runtime_1ga090e14ab721404d80f4404634d5c79cc.md)

    Signed 8-bit integer (-128~127). 

* [using i16 =  std::int16_t](group___runtime_1gaa9061c03e78b5c69a2e90542f956b1b9.md)

    Signed 16-bit integer (-32768~32767). 

* [using i32 =  std::int32_t](group___runtime_1gaec4a1429cc91fb7ff41599b263c348cc.md)

    Signed 32-bit integer (-2147482648~2147483647). 

* [using i64 =  std::int64_t](group___runtime_1gae72e52134285dbd83ca4227ec77394a2.md)

    Signed 64-bit integer (-9223372036854775808~9223372036854775807). 

* [using f32 =  float](group___runtime_1gad34d88453d37b65a09797bad37f2f527.md)

    32-bit (single precision) floating point number. 

* [using f64 =  double](group___runtime_1gabc2f107791bd7c1d49ecf0f168c085a3.md)

    64-bit (double precision) floating point number. 

* [using byte_t =  u8](group___runtime_1gaac1fbcf6f355341ea568024167e570fe.md)
* [using nullptr_t =  std::nullptr_t](group___runtime_1ga7b29db1791dc9e52d93ada17d953ed6d.md)
* [using opaque_t =  void*](group___runtime_1ga1d45eaaf0075f53ddcda26ad3a960faf.md)
* [using c8 =  char](group___runtime_1ga47d3dca6512d0867b2a4126b4643756c.md)

    8-bit character. Signed/unsigned is unspecified, cast this to u8/i8 for fetching number. 

* [using c16 =  char16_t](group___runtime_1gac68b8f40b00545b7c1772fa01931e3c1.md)

    16-bit character. Signed/unsigned is unspecified, cast this to u16/i16 for fetching number. 

* [using c32 =  char32_t](group___runtime_1ga50c94d018de369c551742772ae62d6c9.md)

    32-bit character. Signed/unsigned is unspecified, cast this to u32/i32 for fetching number. 

## Functions
* [constexpr auto test_flags(_Ty flags, _Ty options) -> enable_if_t< is_enum_v< _Ty >, bool >](group___runtime_1ga8199bae21a87e395af52aaa6a96dd16c.md)

    Tests if the provided enumeration contains the specified enumeration option. 

* [constexpr auto set_flags(_Ty &flags, _Ty options) -> enable_if_t< is_enum_v< _Ty >, void >](group___runtime_1ga7f4ce9f18bca2ab726b2c13925d13797.md)

    Sets the provided enumeration options to 1. 

* [constexpr auto reset_flags(_Ty &flags, _Ty options) -> enable_if_t< is_enum_v< _Ty >, void >](group___runtime_1ga6b613b9a6a5376f4ae5ea90d14d310ed.md)

    Resets the provided enumeration options to 0. 

* [constexpr auto set_flags(_Ty flags, _Ty options, bool value) -> enable_if_t< is_enum_v< _Ty >, _Ty >](group___runtime_1gadb531c46cbcfc8f24d9d859afe3cd61c.md)

    Sets the provided enumeration options to 1 or 0 based on the value provided. 

* [auto invoke(_Func &&f) -> decltype(static_cast< _Func && >(f)())](group___runtime_1gaf7411fc1e4c76b86c6f6b69eeb62b704.md)

    Invokes the specified callable object. 

* [auto invoke(_Func &&f, _Ty &&arg1, _Args &&... args) -> invoke_result_t< _Func, _Ty, _Args... >](group___runtime_1gaf7a93152ce0e85bc60d65da9d62c0ca7.md)

    Invokes the specified callable object. 

* [_Return invoke_r(_Func &&f, _Args &&... args)](group___runtime_1gac769aef9bea2b465a9437c25ac6ac9ac.md)

    Invokes the specified callable object. 

* [constexpr ReverseIterator< _Iter > make_reverse_iterator(_Iter i)](group___runtime_1gab53d4c159697d19e8fda0a022d611150.md)

    Creates one reverse iterator from one iterator. 

* [void advance(_Iter &it, _Distance n)](group___runtime_1gaeb004dafbae757b1fe66452065ae8739.md)

    Advances the given iterator by `n` positions respectively. 

* [isize distance(_It first, _It last)](group___runtime_1gacceb07c8bab688f75ae3207dea30f02e.md)

    Gets the number of elements between two iterators. 

* [_Iter next(_Iter it, isize n=1)](group___runtime_1ga4e2d965044b1d306278d256d980423fd.md)

    Gets one iterator pointing to the next `n`th element of the element pointed by the input iterator. 

* [_BidirIt prev(_BidirIt it, isize n=1)](group___runtime_1ga3eab7cd933798dde3a66eb98069ea222.md)

    Gets one iterator pointing to the last `n`th element of the element pointed by the input iterator. 

* [Ref< _Ty > box_ptr(_Ty *obj)](group___runtime_1ga9ffa672f4edd97e1402ea85d169de3aa.md)

    Creates a strong reference from one raw pointer without modifing its reference count. 

* [Ref< _Ty > new_object(_Args &&... args)](group___runtime_1gaa7e539a91bc5a8e68c91db8d2d8a9c23.md)

    Creates one new boxed object. 

