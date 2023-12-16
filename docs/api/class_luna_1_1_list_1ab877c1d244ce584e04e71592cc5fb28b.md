# Luna::List::emplace_back

```c++
template <typename...>
List< _Ty, _Alloc >::reference emplace_back(_Args &&... args)
```

Constructs one element directly on the back of the list using the provided arguments. 



## Parameters
* *in* **args**

    The arguments to construct the element. `_Ty(args...)` will be used to construct the element. 

## Return value
Returns one reference to the constructed element. 

