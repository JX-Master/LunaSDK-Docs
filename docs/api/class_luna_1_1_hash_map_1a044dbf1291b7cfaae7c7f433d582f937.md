# Luna::HashMap::emplace

```c++
template <typename...>
Pair< iterator, bool > emplace(_Args &&... args)
```

Constructs one element directly in the map using the provided arguments. 



## Parameters
* *in* **args**

    The arguments to construct the element. `Pair<const _Kty, _Ty>(args...)` will be used to construct the element. 

## Return value
Returns one iterator-bool pair indicating the result:* If the returned Boolean value is `true`, then the element is successfully constructed and inserted to the map, and the returned iterator points to the inserted element.

* If the returned Boolean value is `false`, then the operation is failed because another element with the same key already exists, and the returned iterator points to the existing element in the map. 

