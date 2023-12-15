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

* [LUNA_RUNTIME_API usize utf8_encode_char(c8 *dst, c32 ch)](group___runtime_unicode_1ga3a868c509b45614efc6f67a97c45ebac.md)

    Encodes the Unicode character into 1~6 UTF-8 characters. 

* [LUNA_RUNTIME_API c32 utf8_decode_char(const c8 *str)](group___runtime_unicode_1ga8ebc9e15201060e9e6765ac7d8fd63dc.md)

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

* [LUNA_RUNTIME_API usize utf16_encode_char(c16 *dst, c32 ch)](group___runtime_unicode_1gae1e4b93bea300345a4c9a39d104c956a.md)

    Encodes the Unicode character into 1~2 UTF-16 characters using platform-native endian. 

* [LUNA_RUNTIME_API c32 utf16_decode_char(const c16 *str)](group___runtime_unicode_1gaeb3a0408fb00d9e81297c1596b8f5205.md)

    Decodes one Unicode character from 1~2 UTF-16 characters. 

* [LUNA_RUNTIME_API usize utf16_to_utf8(c8 *dst, usize dst_max_chars, const c16 *src, usize src_chars=USIZE_MAX)](group___runtime_unicode_1ga616fd70f9d2086579bc2a1a911c60989.md)

    Converts a UTF-16 string to UTF-8 string. 

* [LUNA_RUNTIME_API usize utf16_to_utf8_len(const c16 *src, usize src_chars=USIZE_MAX)](group___runtime_unicode_1ga197d55a887c6b28c409a2e08a8262fce.md)

    Determines the length of the corresponding UTF-8 string for a UTF-16 string, not include the null-terminator. 

* [LUNA_RUNTIME_API usize utf8_to_utf16(c16 *dst, usize dst_max_chars, const c8 *src, usize src_chars=USIZE_MAX)](group___runtime_unicode_1ga69ed8657938fe5dd902db0ca43a7ffac.md)

    Converts a UTF-8 string to UTF-16 string. 

* [LUNA_RUNTIME_API usize utf8_to_utf16_len(const c8 *src, usize src_chars=USIZE_MAX)](group___runtime_unicode_1gaef6da72d8bc9ff2351b9ecd5745f746d.md)

    Determines the length of the corresponding UTF-16 string for a UTF-8 string, not include the null-terminator. 

