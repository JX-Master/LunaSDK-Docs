# Basic types
## Alias types
* [using u8 =  std::uint8_t](group___runtime_base_type_1ga254d32383658e016368673396e7afc1b.md)

    Unsigned 8-bit integer (0~255). 

* [using u16 =  std::uint16_t](group___runtime_base_type_1ga917e58b0692c2df778a27350534cbfe7.md)

    Unsigned 16-bit integer (0~65535). 

* [using u32 =  std::uint32_t](group___runtime_base_type_1ga65cf28726f89e62ccf2f1354bc2716df.md)

    Unsigned 32-bit integer (0~4294967295). 

* [using u64 =  std::uint64_t](group___runtime_base_type_1ga66e1d499241ccae9a18a20a1f4f0590d.md)

    Unsigned 64-bit integer (0~18446744073709551615). 

* [using i8 =  std::int8_t](group___runtime_base_type_1ga090e14ab721404d80f4404634d5c79cc.md)

    Signed 8-bit integer (-128~127). 

* [using i16 =  std::int16_t](group___runtime_base_type_1gaa9061c03e78b5c69a2e90542f956b1b9.md)

    Signed 16-bit integer (-32768~32767). 

* [using i32 =  std::int32_t](group___runtime_base_type_1gaec4a1429cc91fb7ff41599b263c348cc.md)

    Signed 32-bit integer (-2147482648~2147483647). 

* [using i64 =  std::int64_t](group___runtime_base_type_1gae72e52134285dbd83ca4227ec77394a2.md)

    Signed 64-bit integer (-9223372036854775808~9223372036854775807). 

* [using f32 =  float](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md)

    32-bit (single precision) floating point number. 

* [using f64 =  double](group___runtime_base_type_1gabc2f107791bd7c1d49ecf0f168c085a3.md)

    64-bit (double precision) floating point number. 

* [using byte_t =  u8](group___runtime_base_type_1gaac1fbcf6f355341ea568024167e570fe.md)

    An alias of `u8` that represents one byte. You may use this type to differentiate the concept of byte stream (byte_t*) from number array (u8*). 

* [using nullptr_t =  std::nullptr_t](group___runtime_base_type_1ga7b29db1791dc9e52d93ada17d953ed6d.md)

    `usize` is the unsigned integer type of whose length marches the machine architecture. In particular, in 32-bit application, this is 32-bit unsigned integer; in 64-bit application, this is 64-bit unsigned integer. The `usize` type is guaranteed to be large enough to store a indexable memory address, so that any pointer can be reinterpreted casted to `usize`. 

* [using opaque_t =  void*](group___runtime_base_type_1ga1d45eaaf0075f53ddcda26ad3a960faf.md)

    `opaque_t` is used to represent one opaque pointer that shall not be reinterpreted or dereferred by the user. opaque_t are ususally used as arguments or returns values of interface functions to hide the implementation from the user. 

* [using c8 =  char](group___runtime_base_type_1ga47d3dca6512d0867b2a4126b4643756c.md)

    8-bit character. Signed/unsigned is unspecified, cast this to u8/i8 for fetching number. 

* [using c16 =  char16_t](group___runtime_base_type_1gac68b8f40b00545b7c1772fa01931e3c1.md)

    16-bit character. Signed/unsigned is unspecified, cast this to u16/i16 for fetching number. 

* [using c32 =  char32_t](group___runtime_base_type_1ga50c94d018de369c551742772ae62d6c9.md)

    32-bit character. Signed/unsigned is unspecified, cast this to u32/i32 for fetching number. 

## Constants
* [constexpr i8 I8_MAX](group___runtime_base_type_1ga32c5ae73521aeae089b194e8ac50b1a0.md)

    The maximum number that can be represented by one i8 value. 

* [constexpr i8 I8_MIN](group___runtime_base_type_1ga1d49be8662a8526eb5f75e4cdf22aba3.md)

    The minimum number that can be represented by one i8 value. 

* [constexpr i16 I16_MAX](group___runtime_base_type_1ga01d281f806e1c8c16bb124b48494b577.md)

    The maximum number that can be represented by one i16 value. 

* [constexpr i16 I16_MIN](group___runtime_base_type_1ga20261b8d2d35f665533f42d1f6d26820.md)

    The minimum number that can be represented by one i16 value. 

* [constexpr i32 I32_MAX](group___runtime_base_type_1ga2b8c0254aa480505a05869635ff20a22.md)

    The maximum number that can be represented by one i32 value. 

* [constexpr i32 I32_MIN](group___runtime_base_type_1ga3e19e1784153187e88ee245c56c6f571.md)

    The minimum number that can be represented by one i32 value. 

* [constexpr i64 I64_MAX](group___runtime_base_type_1gab02a9a57710d480fd593c00b8d7c71d9.md)

    The maximum number that can be represented by one i64 value. 

* [constexpr i64 I64_MIN](group___runtime_base_type_1gabd21eb34dd9332cb66e64ca7b1aebd47.md)

    The minimum number that can be represented by one i64 value. 

* [constexpr u8 U8_MAX](group___runtime_base_type_1ga13d05fc40e580c724f3408bf319b5d32.md)

    The maximum number that can be represented by one u8 value. 

* [constexpr u16 U16_MAX](group___runtime_base_type_1gadd5a0cc73f6ba243c66a3537361d01f3.md)

    The maximum number that can be represented by one u16 value. 

* [constexpr u32 U32_MAX](group___runtime_base_type_1ga645ed2bd2baa2b4ed82d67bc5597ef47.md)

    The maximum number that can be represented by one u32 value. 

* [constexpr u64 U64_MAX](group___runtime_base_type_1gac5d257d9894ee47f4445391853a0be72.md)

    The maximum number that can be represented by one u64 value. 

* [constexpr usize USIZE_MAX](group___runtime_base_type_1gaf70b42c748a1e2bec2022ea52a74954a.md)

    The maximum number that can be represented by one usize value. 

* [constexpr isize ISIZE_MAX](group___runtime_base_type_1ga6bbaf8e0f5a08b7733d79fdbd836ba4d.md)

    The maximum number that can be represented by one isize value. 

* [constexpr isize ISIZE_MIN](group___runtime_base_type_1ga34b71da9dc525d9f3a36e311383b2c8a.md)

    The minimum number that can be represented by one isize value. 

* [constexpr usize MAX_ALIGN](group___runtime_base_type_1gae771c7d05b7f7738144b784fa44ce6a9.md)

    The maximum alignment requirement for a standard-layout scalar value. 

