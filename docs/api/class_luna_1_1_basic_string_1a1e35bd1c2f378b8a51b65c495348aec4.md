# Luna::BasicString::replace

```c++
void replace(usize pos, usize count, const BasicString &str, usize pos2, usize count2=npos)
```

Replaces characters in range [`pos`, `pos + count`) with a substring [`pos2`, `pos2 + count2`) of `str`. 



## Parameters
* *in* **pos**

    The index of the first character to replace. 

* *in* **count**

    The number of characters to replace. If `pos + count` is greater than `this->size()`, `count` will be clamped to `this->size() - pos`. 

* *in* **str**

    The string to use for replacement. 

* *in* **pos2**

    The index of the first character in `rhs` to use for replacement. 

* *in* **count2**

    The number of characters in `rhs` to use for replacement. If `pos2 + count2` is greater than `str.size()`, `count2` will be clamped to `str.size() - pos2`. 

## Valid Usage
* `pos` must not be greater than `this->size()`.

* `pos2` must not be greater than `str.size()`. 

