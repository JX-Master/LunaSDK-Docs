# Luna::BasicString::BasicString

```c++
BasicString(BasicString &&rhs, const allocator_type &alloc)
```

Constructs one string by moving data from another string. 



## Parameters
* *in* **rhs**

    The string to move data from. This string will be empty after this operation. 

* *in* **alloc**

    The allocator to use. The allocator object will be copy-constructed into the map. 

