# Luna::strstr

```c++
template <typename _CharT>
_CharT * strstr(_CharT *str, const _CharT *substr)
```

Finds the first occurrence of the specified substring in the null-terminated byte string pointed to by `str`. 



## Parameters
* *in* **str**

    The string to be examined. 

* *in* **substr**

    The substring to search for. 

## Return value
Returns one pointer to the first character of the found substring in `str`. Returns `nullptr` if not found. 

## Valid Usage
* Both `str` and `substr` must specify null-terminated strings. 

