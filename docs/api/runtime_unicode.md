# Unicode encoding/decoding
## Functions
* [constexpr usize utf8_charspan(c32 ch)](group___runtime_unicode_1ga38233992601290b6a3bd0fa9699269b4.md)

    Gets the number of UTF-8 characters needed to store the Unicode char in UTF-8 encoding. 

* [constexpr usize utf8_charlen(c8 ch)](group___runtime_unicode_1gac45920bcbff42da3af21f2ef279e535f.md)

    Gets the number of UTF-8 characters the Unicode character takes from the first UTF-8 character. 

* [constexpr usize utf8_charlen(const c8 *src)](group___runtime_unicode_1ga13fea59faaaf664847775a46c6ee809b.md)

    Gets the number of UTF-8 characters the Unicode character takes from the first UTF-8 character. 

* [constexpr usize utf8_strlen(const c8 *src)](group___runtime_unicode_1ga2767a0d4543162786755f0378f95b353.md)

    Gets the number of Unicode characters in a null-terminated UTF-8 string, not including the null terminator. 

* [constexpr usize utf8_index(const c8 *str, usize n)](group___runtime_unicode_1ga184a995230697b71cc1a4ea646f1c3f7.md)

    Gets the index of the first UTF-8 character for the specified Unicode character. 

* [usize utf8_encode_char(c8 *dst, c32 ch)](group___runtime_unicode_1gad7d7f2da8d4e0b42347f65f5b09e9b9c.md)

    Encodes the Unicode character into 1~6 UTF-8 characters. 

* [c32 utf8_decode_char(const c8 *str)](group___runtime_unicode_1ga7668255218e6bb10a3d6434f5465c875.md)

    Decodes one Unicode character from 1~6 UTF-8 characters. 

* [constexpr usize utf16_charspan(c32 ch)](group___runtime_unicode_1gaee1dfeafcf1e5b2e0abfded74899f3c6.md)

    Gets the number of UTF-16 characters needed to store the Unicode char in UTF-16 encoding. 

* [constexpr usize utf16_charlen(c16 ch)](group___runtime_unicode_1gad7b880d245c8ede588b4d269600fb469.md)

    Gets the number of UTF-16 characters the Unicode character takes from the first UTF-16 character. 

* [constexpr usize utf16_charlen(const c16 *src)](group___runtime_unicode_1gafd1e1a65de12a167979bb87b2ed098c6.md)

    Gets the number of UTF-16 characters the Unicode character takes from the first UTF-16 character. 

* [constexpr usize utf16_strlen(const c16 *src)](group___runtime_unicode_1gae4f4c1fac6e2e3e24b751816fbe2c492.md)

    Gets the number of Unicode characters in a null-terminated UTF-16 string, not including the null terminator. 

* [constexpr usize utf16_index(const c16 *str, usize n)](group___runtime_unicode_1ga9ef08852bd4d8cc262fd7d7865647c45.md)

    Gets the index of the first UTF-16 character for the specified Unicode character. 

* [usize utf16_encode_char(c16 *dst, c32 ch)](group___runtime_unicode_1ga8a4f912177e13745d6b347daca9271e3.md)

    Encodes the Unicode character into 1~2 UTF-16 characters using platform-native endian. 

* [c32 utf16_decode_char(const c16 *str)](group___runtime_unicode_1gadd4dba786d538553166c91368a2fbbae.md)

    Decodes one Unicode character from 1~2 UTF-16 characters. 

* [usize utf16_to_utf8(c8 *dst, usize dst_max_chars, const c16 *src, usize src_chars=USIZE_MAX)](group___runtime_unicode_1ga4a6a2af3121c7200e85a617b862d15ea.md)

    Converts a UTF-16 string to UTF-8 string. 

* [usize utf16_to_utf8_len(const c16 *src, usize src_chars=USIZE_MAX)](group___runtime_unicode_1ga65526a3b58a8de0969ad66cfe9327da0.md)

    Determines the length of the corresponding UTF-8 string for a UTF-16 string, not include the null-terminator. 

* [usize utf8_to_utf16(c16 *dst, usize dst_max_chars, const c8 *src, usize src_chars=USIZE_MAX)](group___runtime_unicode_1ga6103c57eaa8e7f268b40ec76d51404f0.md)

    Converts a UTF-8 string to UTF-16 string. 

* [usize utf8_to_utf16_len(const c8 *src, usize src_chars=USIZE_MAX)](group___runtime_unicode_1gad5f06f0a3a8dc6938c4d359f60bfbe74.md)

    Determines the length of the corresponding UTF-16 string for a UTF-8 string, not include the null-terminator. 

