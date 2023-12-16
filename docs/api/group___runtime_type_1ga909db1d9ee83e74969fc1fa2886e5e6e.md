# Luna::hash_func_t

```c++
using hash_func_t =  usize(typeinfo_t type, const void* inst)
```

The hash code computing function used by the reflection system. 



## Parameters
* *in* **type**

    The type of the instance. 

* *in* **inst**

    The pointer to the instance. 

## Return value
Returns the computed hash code. 

