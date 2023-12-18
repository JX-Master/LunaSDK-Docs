# Luna::BasicString::assign

```c++
void assign(const BasicString &str, usize pos, usize count=npos)
```

Assigns the string data by coping characters from one subrange of another string. 



## Parameters
* *in* **str**

    The string to copy characters from. 

* *in* **pos**

    The index of the first character to copy. 

* *in* **count**

    The number of characters to copy. If this is [npos](class_luna_1_1_basic_string_1aba46fb9e7bfa2d6d109cc138bfa6cc11.md), strings in range [`pos`, `str.size()`) will be copied. 

## Valid Usage
* `pos + count` must be not greater than `str.size()`. 

