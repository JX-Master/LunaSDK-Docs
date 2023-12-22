# Luna::BasicString::replace

```c++
template <typename _InputIt>
void replace(const_iterator first, const_iterator last, _InputIt first2, _InputIt last2)
```

Replaces characters in range [`first`, `last`) with the characters in the range [`first2`, `last2`). 



## Parameters
* *in* **first**

    The iterator to the first character to replace. 

* *in* **last**

    The iterator to the one-past-last character to replace. 

* *in* **first2**

    The iterator to the first character to use for replacement. 

* *in* **last2**

    The iterator to the one-past-last character use for replacement. 

## Valid Usage
* [`first`, `last`) must specify a valid range of this string. 

