# Luna::free_library

```c++
LUNA_RUNTIME_API void free_library(opaque_t handle)
```

Unloads the specified library. 



## Parameters
### handle
The library handle returned by load_library. 


When one library is removed from the process's address space, it will decrease reference counters for all its dependent libraries, and removes them as well if their reference counters drop to 0. 

