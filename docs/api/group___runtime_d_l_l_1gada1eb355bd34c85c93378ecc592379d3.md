# Luna::free_library

```c++
void free_library(opaque_t handle)
```

Unloads the specified library. 



## Parameters
* *in* **handle**

    The library handle returned by [load_library](group___runtime_d_l_l_1ga4047beea74e118348cddab00150eb4f8.md). 

## Remark
The library handle is reference counted: every call to [load_library](group___runtime_d_l_l_1ga4047beea74e118348cddab00150eb4f8.md) for the same library file increases the reference counter, and every [free_library](group___runtime_d_l_l_1gada1eb355bd34c85c93378ecc592379d3.md) for the same library handle decreases the reference counter. The library will be removed from the process's address space when the reference counter drop to 0.


When one library is removed from the process's address space, it will decrease reference counters for all its dependent libraries, and removes them as well if their reference counters drop to 0. 

