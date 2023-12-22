# Luna::strlen

```c++
template <typename _CharT>
usize strlen(const _CharT *str)
```

Computes the length (number of characters) of the specified string by searching for the first null character in the string. 



## Parameters
* *in* **str**

    The string to be examined. 

## Return value
Returns the length of the string. The length does not include the null terminator. 

## Valid Usage
* `str` must specify one null-terminated string. 

