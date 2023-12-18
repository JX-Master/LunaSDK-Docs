# Luna::BasicString::BasicString

```c++
BasicString(const value_type *s, usize count, const allocator_type &alloc=allocator_type())
```

Constructs one string by coping characters from the provided character array. 



## Parameters
* *in* **s**

    The pointer to the first character to copy. 

* *in* **count**

    The number of characters to copy. 

* *in* **alloc**

    The allocator to use. The allocator object will be copy-constructed into the map. 

## Valid Usage
* If `count` is not `0`, `s` must points to a valid character array with at least `count` characters. 

