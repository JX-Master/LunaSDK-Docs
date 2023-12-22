# String library
## Types
* [Luna::BasicString](class_luna_1_1_basic_string.md)

    The basic string implementation that is suitable for any character types. 


## Alias types
* [using String =  BasicString<c8>](group___runtime_string_1ga23546c7e0a7ea4a45e5cf5beb6cac680.md)

    The string that contains [c8](group___runtime_base_type_1ga47d3dca6512d0867b2a4126b4643756c.md) characters. 

* [using WString =  BasicString<wchar_t>](group___runtime_string_1ga08f6060c714d7fa04b579914c22f3125.md)

    The string that contains wchat_t characters. 

* [using String16 =  BasicString<c16>](group___runtime_string_1gac9b90cbbafc1e42b8e307653110f875e.md)

    The string that contains [c16](group___runtime_base_type_1gac68b8f40b00545b7c1772fa01931e3c1.md) characters. 

* [using String32 =  BasicString<c32>](group___runtime_string_1ga41c692c42804b8cea95cbfd865d8c188.md)

    The string that contains [c32](group___runtime_base_type_1ga50c94d018de369c551742772ae62d6c9.md) characters. 

## Functions
* [typeinfo_t string_type()](group___runtime_string_1ga3d4128790c1939189bff135a3ed42f31.md)

    Gets the type object of [String](group___runtime_string_1ga23546c7e0a7ea4a45e5cf5beb6cac680.md). 

* [usize strlen(const _CharT *str)](group___runtime_string_1gacabe981ca12e2bfa89fc57ca022360a5.md)

    Computes the length (number of characters) of the specified string by searching for the first null character in the string. 

* [usize strnlen(const _CharT *str, usize max_chars)](group___runtime_string_1gaef8e21f38a901af5e7e1560fef08fe53.md)

    Computes the length (number of characters) of the specified string by searching for the first null character in the string. The search process stops after reading `max_chars` characters. 

* [_CharT * strncpy(_CharT *dst, const _CharT *src, usize max_chars)](group___runtime_string_1gaf12851566cf848485c57fcbfaa1f2a15.md)

    Copies at most `max_chars` characters from `src` to `dst`, including the null terminator. 

* [i32 strcmp(const _CharT *lhs, const _CharT *rhs)](group___runtime_string_1ga9904129fec4d472dc56e5d4466606b75.md)

    Compares characters in two strings. 

* [i32 strncmp(const _CharT *lhs, const _CharT *rhs, usize max_chars)](group___runtime_string_1ga42318bd6d6007b678467563e35ece712.md)

    Compares at most `max_chars` characters in two strings. 

* [const _CharT * strchr(const _CharT *str, _CharT ch)](group___runtime_string_1gadd592bd562db4e26e8f238464a95c594.md)

    Finds the first occurrence of `ch` in the null-terminated byte string pointed to by `str`. 

* [_CharT * strchr(_CharT *str, _CharT ch)](group___runtime_string_1ga9c63f4e45c5f8ae2f96fa5a1ce751a8a.md)

    Finds the first occurrence of `ch` in the null-terminated byte string pointed to by `str`. 

* [const _CharT * strrchr(const _CharT *str, _CharT ch)](group___runtime_string_1ga609822553b70c66ca522ac3eea71eefd.md)

    Finds the last occurrence of `ch` in the null-terminated byte string pointed to by `str`. 

* [_CharT * strrchr(_CharT *str, _CharT ch)](group___runtime_string_1gada1de36e8ded52db5177c3e382c04844.md)

    Finds the last occurrence of `ch` in the null-terminated byte string pointed to by `str`. 

* [const _CharT * strstr(const _CharT *str, const _CharT *substr)](group___runtime_string_1ga58caa8c31ce8a13b0d0e87eb71e519a4.md)

    Finds the first occurrence of the specified substring in the null-terminated byte string pointed to by `str`. 

* [_CharT * strstr(_CharT *str, const _CharT *substr)](group___runtime_string_1ga8c1b4fc1a110caeb47fbb0425d56e5a7.md)

    Finds the first occurrence of the specified substring in the null-terminated byte string pointed to by `str`. 

* [i64 strtoi64(const c8 *str, c8 **str_end, i32 base)](group___runtime_string_1gabce39c59b3d2a2032606aac06f3469a0.md)

    Interprets an integer value in a string pointed to by `str`. 

* [u64 strtou64(const c8 *str, c8 **str_end, i32 base)](group___runtime_string_1ga2bff2dfad090afc178aa5ee90980e944.md)

    Interprets an unsigned integer value in a string pointed to by `str`. 

* [f64 strtof64(const c8 *str, c8 **str_end)](group___runtime_string_1ga1dc74e0088745a1dcab1380dce047be2.md)

    Interprets a floating-point value in a string pointed to by `str`. 

* [f32 strtof32(const c8 *str, c8 **str_end)](group___runtime_string_1ga6d12249821d3f0232b68eb551b97fcee.md)

    Interprets a floating-point value in a string pointed to by `str`. 

