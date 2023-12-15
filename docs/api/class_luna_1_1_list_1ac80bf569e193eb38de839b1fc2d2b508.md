# Luna::List::emplace_front

```c++
template <typename...>
List< _Ty, _Alloc >::reference emplace_front(_Args &&... args)
```

Constructs one element directly on the front of the list using the provided arguments. 



## Parameters
### args
The arguments to construct the element. `_Ty(args...)` will be used to construct the element. 

## Return value
Returns one reference to the constructed element. 

