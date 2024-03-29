# Luna::base85_encode

```c++
usize base85_encode(c8 *dst, usize dst_max_chars, const void *src, usize src_size_bytes)
```

Encode a binary data to a base85 string. 



## Parameters
* *in* **dst**

    The character buffer used to hold the encoded base85 string. 

* *in* **dst_max_chars**

    The maximum characters the `dst` buffer can hold, including the null-terminator. 

* *in* **src**

    The source binary data. 

* *in* **src_size_bytes**

    The size of the source binary data in bytes. 

## Return value
Returned the number of characters outputted into `dst` buffer. 

## Valid Usage
* If `src_size_bytes` is not `0`, `src_size_bytes` must be times of 4. 

