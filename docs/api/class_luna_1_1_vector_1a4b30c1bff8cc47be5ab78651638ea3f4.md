# Luna::Vector::Vector

```c++
template <typename _InputIt>
Vector(enable_if_t<!is_integral_v< _InputIt >, _InputIt > first, _InputIt last, const allocator_type &alloc=allocator_type())
```

Constructs one vector with elements copied from the specified range. 



## Parameters
* *in* **first**

    The iterator that points to the first element of the copy range. 

* *in* **last**

    The iterator that points to the last element of the copy range. 

* *in* **alloc**

    The optioanl allocator instance bound to this vector. The allocator instance is copied into the vector type.


This function creates a vector whose elements are copied from range `[first, last)`, the iterator parameters should support be input iterators. 

