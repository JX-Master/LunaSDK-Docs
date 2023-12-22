# Luna::BasicString::replace

```c++
void replace(usize pos, usize count, const BasicString &str)
```

Replaces characters in range [`pos`, `pos + count`) with characters of `str`. 



## Parameters
* *in* **pos**

    The index of the first character to replace. 

* *in* **count**

    The number of characters to replace. If `pos + count` is greater than `this->size()`, `count` will be clamped to `this->size() - pos`. 

* *in* **str**

    The string to use for replacement. 

## Valid Usage
* `pos` must not be greater than `this->size()`. 

