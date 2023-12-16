# Luna::free_library

```c++
void free_library(opaque_t handle)
```

Unloads the specified library. 



## Parameters
### handle
The library handle returned by [load_library](group___runtime_d_l_l_1gaf089b17ba5687b844e5ab7233a65a24e.md). 

## Remark
The library handle is reference counted: every call to [load_library](group___runtime_d_l_l_1gaf089b17ba5687b844e5ab7233a65a24e.md) for the same library file increases the reference counter, and every [free_library](group___runtime_d_l_l_1gaeb0bf745d9d2223a5b090a394d686164.md) for the same library handle decreases the reference counter. The library will be removed from the process's address space when the reference counter drop to 0.


When one library is removed from the process's address space, it will decrease reference counters for all its dependent libraries, and removes them as well if their reference counters drop to 0. 

