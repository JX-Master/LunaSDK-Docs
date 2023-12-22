# Luna::BasicString::substr

```c++
BasicString< _Char, _Alloc > substr(usize pos=0, usize count=npos) const
```

Creates a substring of this string. 



## Parameters
* *in* **pos**

    The index of the first character to include in the substring. 

* *in* **count**

    The number of characters to include in the substring. If `pos + count` is greater than `this->size()`, `count` will be clamped to `this->size() - pos`. 

## Return value
Returns the created substring. 

## Valid Usage
* `pos` must not be greater than `this->size()`. 

