# Luna::utf8_to_utf16

```c++
usize utf8_to_utf16(c16 *dst, usize dst_max_chars, const c8 *src, usize src_chars=USIZE_MAX)
```

Converts a UTF-8 string to UTF-16 string. 



## Parameters
* *in* **dst**

    The buffer to hold the output string. 

* *in* **dst_max_chars**

    The maximum characters the `dst` buffer can hold, including the null-terminator. 

* *in* **src**

    The holding the source string. 

* *in* **src_chars**

    The maximum characters to read. Specify `USIZE_MAX` to read till the end of the string. The conversion process will stop on first null terminator, or when `src_chars` is reached. 

## Return value
Returns the number of characters outputted to the `dst` buffer, not including the null-terminator. 

## Valid Usage
* `src` must be a valid UTF-8 string. 

