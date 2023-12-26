# Luna::Vector::resize

```c++
void resize(usize n, const value_type &v)
```

Resizes the vector. 

If the new size is greater than [size](class_luna_1_1_vector_1a79348f1b7c06b34052b42656a0279429.md), new elements will be copy-inserted at the back of the vector using the provided value.

If the new size is smaller than [size](class_luna_1_1_vector_1a79348f1b7c06b34052b42656a0279429.md), `size - n` elements will be removed from the back of the vector.

If the new size is equal to [size](class_luna_1_1_vector_1a79348f1b7c06b34052b42656a0279429.md), this function does nothing. 

## Parameters
* *in* **n**

    The new size of the vector. 

* *in* **v**

    The initial value to copy for new elements. 

