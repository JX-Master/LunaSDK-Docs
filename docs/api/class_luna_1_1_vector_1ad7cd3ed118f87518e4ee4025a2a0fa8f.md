# Luna::Vector::erase

```c++
Vector< _Ty, _Alloc >::iterator erase(const_iterator pos)
```

Removes one element from the vector. 



## Parameters
* *in* **pos**

    The iterator to the element to be removed. 

## Return value
Returns one iterator to the next element after the removed element, or `end()` if such element does not exist. 

## Valid Usage
* `pos` must points to a valid element in the vector. 

