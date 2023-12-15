# Base64 encoding/decoding
## Functions
* [constexpr usize base64_get_encoded_size(usize raw_size)](group___runtime_base64_1gaa0d5ab0bffe4d19bffec6e45286e35e4.md)

    Get the encoded base64 string size from the raw data size. 

* [constexpr usize base64_get_decoded_size(usize encoded_size)](group___runtime_base64_1ga0e46b91bd3c086745a6704a189fada6f.md)

    Get the decoded binary size from the encoded base64 string size. 

* [LUNA_RUNTIME_API usize base64_encode(c8 *dst, usize dst_max_chars, const void *src, usize src_size_bytes)](group___runtime_base64_1gac35704080d8056581fa46d6098112ca1.md)

    Encode a binary data to a base64 string. 

* [LUNA_RUNTIME_API usize base64_decode(void *dst, usize dst_max_bytes, const c8 *src, usize src_size_chars=USIZE_MAX)](group___runtime_base64_1gab65c5e01817dfa051460e90392b09b1f.md)

    Decode a base64 string to binary data. The system assumes the string passed in is a valid base64 string. 

