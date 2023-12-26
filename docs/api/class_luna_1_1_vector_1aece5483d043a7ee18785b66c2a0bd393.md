# Luna::Vector::Vector

```c++
Vector(usize count, const value_type &value, const allocator_type &alloc=allocator_type())
```

Constructs one vector with `count` elements, with their values initialized by `value`. 



## Parameters
* *in* **count**

    The number of elements in the vector. 

* *in* **value**

    The value for each element in the vector. The value is copy constructed into each element. 

* *in* **alloc**

    The optioanl allocator instance bound to this vector. The allocator instance is copied into the vector type. 

