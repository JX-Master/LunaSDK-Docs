# Luna::BasicString::find

```c++
usize find(const BasicString &str, usize pos=0) const
```

Finds the first occurrence of the specified character sequence in the string. 



## Parameters
* *in* **str**

    The string that holds the character sequence to search. 

* *in* **pos**

    The index at which to start the search. 

## Return value
Returns the index of the first character of the found occurrence. Returns [npos](class_luna_1_1_basic_string_1aba46fb9e7bfa2d6d109cc138bfa6cc11.md) if no such occurrence is found. 

