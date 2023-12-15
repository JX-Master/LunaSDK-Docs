# Luna::memory_profiler_set_memory_type

```c++
LUNA_RUNTIME_API void memory_profiler_set_memory_type(void *ptr, const c8 *type, usize str_size=USIZE_MAX)
```

Sets the type of the object this memory block. 



## Parameters
### ptr
The memory block pointer. 

### domain
The type name for the memory block. 

### str_size
The size of the name, not including the null terminator. If this is `USIZE_MAX`, the size is determined by the system using strlen. 

