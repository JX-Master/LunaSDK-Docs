# Luna::BasicString::BasicString

```c++
BasicString(const value_type *s, const allocator_type &alloc=allocator_type())
```

Constructs one string by coping characters from the provided null-terminated C string. The length of the string is determined by the first null character. 



## Parameters
* *in* **s**

    The pointer to one null-terminated string, where characters are copied from. 

* *in* **alloc**

    The allocator to use. The allocator object will be copy-constructed into the map. 

## Valid Usage
* `s` must points to a valid null-terminated string. 

