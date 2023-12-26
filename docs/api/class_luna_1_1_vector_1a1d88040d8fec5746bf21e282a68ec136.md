# Luna::Vector::emplace_back

```c++
template <typename...>
Vector< _Ty, _Alloc >::iterator emplace_back(_Args &&... args)
```

Constructs one element directly on the back of the vector using the provided arguments. 



## Parameters
* *in* **args**

    The arguments to construct the element. `_Ty(args...)` will be used to construct the element. 

## Return value
Returns one reference to the constructed element. 

