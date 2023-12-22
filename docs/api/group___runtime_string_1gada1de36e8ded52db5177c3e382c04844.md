# Luna::strrchr

```c++
template <typename _CharT>
_CharT * strrchr(_CharT *str, _CharT ch)
```

Finds the last occurrence of `ch` in the null-terminated byte string pointed to by `str`. 

The terminating null character is considered to be a part of the string and can be found if searching for `\0`. 

## Parameters
* *in* **str**

    The string to be examined. 

* *in* **ch**

    The character to search for. 

## Return value
Returns one pointer to the found character in `str`. Returns `nullptr` if not found. 

## Valid Usage
* `str` must specify one null-terminated string. 

