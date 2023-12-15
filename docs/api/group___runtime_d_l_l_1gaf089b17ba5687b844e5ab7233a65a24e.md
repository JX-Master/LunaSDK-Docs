# Luna::load_library

```c++
LUNA_RUNTIME_API R< opaque_t > load_library(const c8 *path)
```

Loads the specified library to the process's address space. This call may load additional libraries required by the specified library. 



## Parameters
### path
The path of the library file. It can be one `.dll` or `.exe` file on Windows, or one `.so` file on POSIX systems. 

## Return value
Returns one handle that represents the loaded library. 

