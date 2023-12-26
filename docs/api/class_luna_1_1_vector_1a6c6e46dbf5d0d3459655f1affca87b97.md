# Luna::Vector::Vector

```c++
Vector(Vector &&rhs, const allocator_type &alloc)
```

Constructs a vector with an custom allocator and with elements moved from another vector. 



## Parameters
* *in* **rhs**

    The vector to move elements from. 

* *in* **alloc**

    The allocator to use. The allocator object will be copy-constructed into the vector. 

