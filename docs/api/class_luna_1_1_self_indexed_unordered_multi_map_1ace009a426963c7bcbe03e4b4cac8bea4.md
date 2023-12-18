# Luna::SelfIndexedUnorderedMultiMap::emplace

```c++
template <typename...>
iterator emplace(_Args &&... args)
```

Constructs one element directly in the map using the provided arguments. 



## Parameters
* *in* **args**

    The arguments to construct the element. `_Ty(args...)` will be used to construct the element. 

## Return value
Returns one iterator to the inserted element. 

