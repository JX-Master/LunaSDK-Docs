# Luna::utf16_to_utf8

```c++
usize utf16_to_utf8(c8 *dst, usize dst_max_chars, const c16 *src, usize src_chars=USIZE_MAX)
```

Converts a UTF-16 string to UTF-8 string. 



## Parameters
* *in* **dst**

    The buffer to hold the output string. 

* *in* **dst_max_chars**

    The maximum characters the `dst` buffer can hold, including the null-terminator. 

* *in* **src**

    The buffer holding the source string. 

* *in* **src_chars**

    The maximum characters to read. Specify `USIZE_MAX` to read till the end of the string. The conversion process will stop on first null terminator, or when `src_chars` is reached. 

## Return value
Returns the number of characters outputted to the `dst` buffer, not including the null-terminator. 

## Valid Usage
* `src` must be a valid UTF-16 string. 

