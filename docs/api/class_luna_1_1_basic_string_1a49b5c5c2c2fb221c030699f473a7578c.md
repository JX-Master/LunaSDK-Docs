# Luna::BasicString::copy

```c++
usize copy(value_type *dst, usize count, usize pos=0) const
```

Copies a substring [`pos`, `pos + count`) to character string pointed to by `dst`. 



## Parameters
* *in* **dst**

    The pointer to the destination character string. 

* *in* **count**

    The number of characters to copy. If `pos + count` is greater than `this->size()`, `count` will be clamped to `this->size() - pos`. 

* *in* **pos**

    The index of the first character to copy. 

## Return value
Returns number of characters copied. 

## Valid Usage
* `pos` must not be greater than `this->size()`. 

