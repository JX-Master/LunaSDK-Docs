# Luna::Vector::back

```c++
Vector< _Ty, _Alloc >::const_reference back() const
```

Gets the element at the back of the vector. 

The back element is the element with index `size() - 1`. 

## Return value
Returns one constant reference to the back element of the vector. 

## Valid Usage
* [empty](class_luna_1_1_vector_1a644718bb2fb240de962dc3c9a1fdf0dc.md) must be `false` when calling this function. 

