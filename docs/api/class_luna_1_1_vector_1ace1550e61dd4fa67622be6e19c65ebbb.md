# Luna::Vector::at

```c++
Vector< _Ty, _Alloc >::const_reference at(usize n) const
```

Gets the element at the specified index. 



## Parameters
* *in* **n**

    The index of the element. 

## Return value
Returns one reference to the element at the specified index. 

## Valid Usage
* [empty](class_luna_1_1_vector_1a644718bb2fb240de962dc3c9a1fdf0dc.md) must be `false` when calling this function.

* `n` must be in range [`0`, `size()`). 

