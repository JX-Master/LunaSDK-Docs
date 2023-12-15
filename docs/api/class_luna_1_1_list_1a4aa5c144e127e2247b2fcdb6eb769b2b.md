# Luna::List::emplace

```c++
template <typename...>
List< _Ty, _Alloc >::iterator emplace(const_iterator pos, _Args &&... args)
```

Constructs one element directly on the specified position of the list using the provided arguments. 

## Overview


## Parameters
### pos
The iterator pointing to the position to construct the element. The elements will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the list. 

### args
The arguments to construct the element. `_Ty(args...)` will be used to construct the element. 

## Return value
Returns one iterator pointing to the constructed element. 

