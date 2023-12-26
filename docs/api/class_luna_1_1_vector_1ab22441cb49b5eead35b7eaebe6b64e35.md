# Luna::Vector::emplace

```c++
template <typename...>
Vector< _Ty, _Alloc >::iterator emplace(const_iterator pos, _Args &&... args)
```

Constructs one element directly on the specified position of the vector using the provided arguments. 



## Parameters
* *in* **pos**

    The iterator to the position to construct the element. The elements will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the vector. 

* *in* **args**

    The arguments to construct the element. `_Ty(args...)` will be used to construct the element. 

## Return value
Returns one iterator to the constructed element. 

