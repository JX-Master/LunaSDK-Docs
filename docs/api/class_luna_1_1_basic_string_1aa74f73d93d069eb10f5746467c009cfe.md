# Luna::BasicString::replace

```c++
void replace(usize pos, usize count, usize count2, value_type ch)
```

Replaces characters in range [`pos`, `pos + count`) with `count2` copies of character `ch`. 



## Parameters
* *in* **pos**

    The index of the first character to replace. 

* *in* **count**

    The number of characters to replace. If `pos + count` is greater than `this->size()`, `count` will be clamped to `this->size() - pos`. 

* *in* **count2**

    The number of characters to use for replacement. 

* *in* **ch**

    The character to use for replacement. 

## Valid Usage
* `pos` must not be greater than `this->size()`. 

