# Luna::BasicString::BasicString

```c++
BasicString(const BasicString &rhs, usize pos, usize count, const allocator_type &alloc=allocator_type())
```

Constructs one string by coping characters from another string. 



## Parameters
* *in* **rhs**

    The string to copy from. 

* *in* **pos**

    The index of the first character to copy. 

* *in* **count**

    The number of characters to copy. Characters in range [`pos`, `pos + count`) of `rhs` will be copied. 

* *in* **alloc**

    The allocator to use. The allocator object will be copy-constructed into the map. 

## Valid Usage
* `pos + count` must be not greater than `rhs.size()`. 

