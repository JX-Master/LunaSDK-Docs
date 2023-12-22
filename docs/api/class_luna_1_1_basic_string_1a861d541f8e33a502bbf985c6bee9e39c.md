# Luna::BasicString::replace

```c++
void replace(const_iterator first, const_iterator last, usize count2, value_type ch)
```

Replaces characters in range [`first`, `last`) with `count2` copies of character `ch`. 



## Parameters
* *in* **first**

    The iterator to the first character to replace. 

* *in* **last**

    The iterator to the one-past-last character to replace. 

* *in* **count2**

    The number of characters to use for replacement. 

* *in* **ch**

    The character to use for replacement. 

## Valid Usage
* [`first`, `last`) must specify a valid range of this string. 

