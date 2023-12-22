# Luna::BasicString::replace

```c++
void replace(const_iterator first, const_iterator last, const BasicString &str)
```

Replaces characters in range [`first`, `last`) with characters of `str`. 



## Parameters
* *in* **first**

    The iterator to the first character to replace. 

* *in* **last**

    The iterator to the one-past-last character to replace. 

* *in* **str**

    The string to use for replacement. 

## Valid Usage
* [`first`, `last`) must specify a valid range of this string. 

