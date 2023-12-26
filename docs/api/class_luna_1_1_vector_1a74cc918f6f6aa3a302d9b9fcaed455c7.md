# Luna::Vector::Vector

```c++
Vector(InitializerList< value_type > init, const allocator_type &alloc=allocator_type())
```

Constructs one vector by coping all elements from an initializer list. 



## Parameters
* *in* **init**

    The initializer list that contains the initial data of the vector. Every element of the new vector is copy-constructed from the corresponding elements in the initializer list. 

* *in* **alloc**

    The optioanl allocator instance bound to this vector. The allocator instance is copied into the vector type. 

