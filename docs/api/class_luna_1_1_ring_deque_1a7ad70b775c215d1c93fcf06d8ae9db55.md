# Luna::RingDeque::emplace_front

```c++
template <typename...>
iterator emplace_front(_Args &&... args)
```

Constructs one element directly on the front of the queue using the provided arguments. 



## Parameters
* *in* **args**

    The arguments to construct the element. `_Ty(args...)` will be used to construct the element. 

## Return value
Returns one reference to the constructed element. 

