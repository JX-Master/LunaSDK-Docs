# Luna::BasicString::replace

```c++
void replace(const_iterator first, const_iterator last, const value_type *cstr)
```

Replaces characters in range [`first`, `last`) with a null-terminated C string. 



## Parameters
* *in* **first**

    The iterator to the first character to replace. 

* *in* **last**

    The iterator to the one-past-last character to replace. 

* *in* **cstr**

    The pointer to the null-terminated C string to use for replacement. 

## Valid Usage
* [`first`, `last`) must specify a valid range of this string.

* `cstr` must points to a valid null-terminated string. 

