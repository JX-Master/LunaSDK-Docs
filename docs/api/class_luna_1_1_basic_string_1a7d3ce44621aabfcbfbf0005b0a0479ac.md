# Luna::BasicString::rfind

```c++
usize rfind(const value_type *s, usize pos=0) const
```

Finds the last occurrence of the specified character sequence in the string. 



## Parameters
* *in* **s**

    The string that holds the character sequence to search. Characters in range [`s`, `s + strlen(s)`) will be used for searching. 

* *in* **pos**

    The index at which to begin searching. The character at `pos` is included in searching. If `pos >= size()` (including [npos](class_luna_1_1_basic_string_1aba46fb9e7bfa2d6d109cc138bfa6cc11.md)), the search will start from the end of the string. 

## Return value
Returns the index of the first character of the found occurrence. The index is an offset from the start of the string, not the end. Returns [npos](class_luna_1_1_basic_string_1aba46fb9e7bfa2d6d109cc138bfa6cc11.md) if no such occurrence is found.


If `strlen(s)` is `0`, returns `pos` if `pos < size()`, returns `size()` otherwise.

[npos](class_luna_1_1_basic_string_1aba46fb9e7bfa2d6d109cc138bfa6cc11.md) is always returned if `size() == 0`, even if `strlen(s)` is `0`. 

## Valid Usage
* `s` must points to a valid null-terminated string. 

