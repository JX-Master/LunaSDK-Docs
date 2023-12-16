# Luna::base64_decode

```c++
usize base64_decode(void *dst, usize dst_max_bytes, const c8 *src, usize src_size_chars=USIZE_MAX)
```

Decode a base64 string to binary data. The system assumes the string passed in is a valid base64 string. 



## Parameters
* *in* **dst**

    The binary buffer used to hold the decoded data. 

* *in* **dst_max_bytes**

    The maximum bytes the `dst` buffer can hold. 

* *in* **src**

    The null-terminated base64 source string. 

* *in* **src_size_chars**

    The maximum characters to read in the `src` string. Specify `USIZE_MAX` to read the full string. 

## Return value
Returns the number of bytes decoded into the `dst` buffer. 

