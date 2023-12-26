# Luna::Vector::swap_erase

```c++
Vector< _Ty, _Alloc >::iterator swap_erase(const_iterator pos)
```

Destructs the element at specified posiiton, then relocates the last element of the vector to the specified position. 

This can be used to prevent moving elements when the element order is not significant. 

## Parameters
* *in* **pos**

    The iterator to the element to be removed. 

## Return value
Returns one iterator to the next element after the removed element, or `end()` if such element does not exist. 

## Valid Usage
* `pos` must points to a valid element in the vector. 

