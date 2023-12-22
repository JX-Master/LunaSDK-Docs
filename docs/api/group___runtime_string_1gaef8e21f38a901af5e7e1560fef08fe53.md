# Luna::strnlen

```c++
template <typename _CharT>
usize strnlen(const _CharT *str, usize max_chars)
```

Computes the length (number of characters) of the specified string by searching for the first null character in the string. The search process stops after reading `max_chars` characters. 



## Parameters
* *in* **str**

    The string to be examined. 

* *in* **max_chars**

    The maximum number of characters to examine, including the null terminator. 

## Return value
Returns the length of the string. The length does not include the null terminator. Returns `0` if `s` is `nullptr`. Returns `max_chars` if the null character is not found in the first `max_chars` characters of `s`. 

