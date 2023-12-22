# Luna::BasicString::rfind

```c++
usize rfind(value_type ch, usize pos=npos) const
```

Finds the first occurrence of the specified character in the string. 



## Parameters
* *in* **ch**

    The character to search for. 

* *in* **pos**

    The index at which to begin searching. The character at `pos` is included in searching. If `pos >= size()` (including [npos](class_luna_1_1_basic_string_1aba46fb9e7bfa2d6d109cc138bfa6cc11.md)), the search will start from the end of the string. 

## Return value
Returns the index of the found character. Returns [npos](class_luna_1_1_basic_string_1aba46fb9e7bfa2d6d109cc138bfa6cc11.md) if no such occurrence is found. 

