# Luna::BasicString::find

```c++
usize find(const value_type *s, usize pos, usize count) const
```

Finds the first occurrence of the specified character sequence in the string. 



## Parameters
* *in* **s**

    The string that holds the character sequence to search. 

* *in* **pos**

    The index at which to start the search. 

* *in* **count**

    The number of characters to search. Character in range [`s`, `s + count`) will be used for searching. 

## Return value
Returns the index of the first character of the found occurrence. Returns [npos](class_luna_1_1_basic_string_1aba46fb9e7bfa2d6d109cc138bfa6cc11.md) if no such occurrence is found. 

