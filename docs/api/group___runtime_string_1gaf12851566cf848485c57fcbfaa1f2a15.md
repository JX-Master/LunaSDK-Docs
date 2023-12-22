# Luna::strncpy

```c++
template <typename _CharT>
_CharT * strncpy(_CharT *dst, const _CharT *src, usize max_chars)
```

Copies at most `max_chars` characters from `src` to `dst`, including the null terminator. 

The real number of characters copied from `src` will be `min(max_chars - 1, strlen(dst))`. The null terminator will then be written at the end of the copied characters. 

## Parameters
* *in* **dst**

    The character buffer to copy to. 

* *in* **src**

    The character buffer to copy from. 

* *in* **max_chars**

    The maximum number of characters that can be written to `dst`, including the null terminator. 

## Return value
Returns `dst`. 

