# Luna::BasicString::replace

```c++
void replace(usize pos, usize count, const value_type *cstr)
```

Replaces characters in range [`pos`, `pos + count`) with a null-terminated C string. 



## Parameters
* *in* **pos**

    The index of the first character to replace. 

* *in* **count**

    The number of characters to replace. If `pos + count` is greater than `this->size()`, `count` will be clamped to `this->size() - pos`. 

* *in* **cstr**

    The pointer to the null-terminated C string to use for replacement. 

## Valid Usage
* `pos` must not be greater than `this->size()`.

* `cstr` must points to a valid null-terminated string. 

