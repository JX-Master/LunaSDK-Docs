# Base85 encoding/decoding
## Functions
* [constexpr usize base85_get_encoded_size(usize raw_size)](group___runtime_base85_1ga179de9a75197a8f4081eda479c009543.md)

    Get the encoded base85 string size from the raw data size. 

* [constexpr usize base85_get_decoded_size(usize encoded_size)](group___runtime_base85_1ga06671340e30506df9cc9c7ed35009bdd.md)

    Get the decoded binary size from the encoded base85 string size. 

* [LUNA_RUNTIME_API usize base85_encode(c8 *dst, usize dst_max_chars, const void *src, usize src_size_bytes)](group___runtime_base85_1gad78cb4c9aa1e3efed5ba6aa94a26b473.md)

    Encode a binary data to a base85 string. 

* [LUNA_RUNTIME_API usize base85_decode(void *dst, usize dst_max_bytes, const c8 *src, usize src_size_chars=USIZE_MAX)](group___runtime_base85_1gae83719ffcccb1216cbaf51c6ecd3a302.md)

    Decode a base85 string to binary data. The system assumes the string passed in is a valid base85 string. 

