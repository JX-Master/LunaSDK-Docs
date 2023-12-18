# Luna::BasicString::BasicString

```c++
BasicString(const BasicString &rhs, usize pos, const allocator_type &alloc=allocator_type())
```

Constructs one string by coping characters in range from another string. 



## Parameters
* *in* **rhs**

    The string to copy from. 

* *in* **pos**

    The index of the first character to copy. Characters in range [`pos`, `rhs.size()`) of `rhs` will be copied. 

* *in* **alloc**

    The allocator to use. The allocator object will be copy-constructed into the map. 

## Valid Usage
* `pos` must be smaller than `rhs.size()`. 

