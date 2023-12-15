# Luna::base64_get_decoded_size

```c++
constexpr usize base64_get_decoded_size(usize encoded_size)
```

Get the decoded binary size from the encoded base64 string size. 

This value may be greater than the actual data size if the size of raw data is not times of 3. You should use this value to allocate memory, and use the size value returned by the actual decode function as the size information, since that is precise. 

## Parameters
### encoded_size
The size of the encoded string, in bytes, and not including the null terminator. 

## Return value
The size of the decoded raw data, in bytes. 

