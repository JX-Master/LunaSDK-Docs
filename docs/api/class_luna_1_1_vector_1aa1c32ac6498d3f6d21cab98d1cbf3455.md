# Luna::Vector::reserve

```c++
void reserve(usize new_cap)
```

Increases the capacity of the vector to a value greater than or equal to `new_cap`, so that it can hold at least `new_cap` elements without reallocating the internal buffer. 

If `new_cap` is smaller than or equal to [capacity](class_luna_1_1_vector_1ad96bf59cb22e917cbd210ba068e8acb3.md), this function does nothing. 

## Parameters
* *in* **new_cap**

    The new capacity value to reserve. 

