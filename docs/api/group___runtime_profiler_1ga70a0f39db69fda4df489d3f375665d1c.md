# Luna::memory_profiler_set_memory_name

```c++
void memory_profiler_set_memory_name(void *ptr, const c8 *name, usize str_size=USIZE_MAX)
```

Sets a debug name for the memory block, for example, the name of the resource file this memory block is allocated for. This function emits one PROFILER_EVENT_ID_SET_MEMORY_NAME profiler event. 



## Parameters
### ptr
The memory block pointer. 

### name
The debug name for the memory block. 

### str_size
The size of the name, not including the null terminator. If this is `USIZE_MAX`, the size is determined by the system using strlen. 

