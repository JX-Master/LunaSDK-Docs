# Luna::base85_decode

```c++
LUNA_RUNTIME_API usize base85_decode(void *dst, usize dst_max_bytes, const c8 *src, usize src_size_chars=USIZE_MAX)
```

Decode a base85 string to binary data. The system assumes the string passed in is a valid base85 string. 



## Parameters
### dst
The binary buffer used to hold the decoded data. 

### dst_max_bytes
The maximum bytes the `dst` buffer can hold. 

### src
The null-terminated base85 source string. 

### src_size_chars
The maximum characters to read in the `src` string. Specify `USIZE_MAX` to read the full string. 

## Return value
Returns the number of bytes decoded into the `dst` buffer. 

#### Valid Usage
* If `src_size_bytes` is neither `0` nor `USIZE_MAX`, `src_size_bytes` must be times of 5. 

