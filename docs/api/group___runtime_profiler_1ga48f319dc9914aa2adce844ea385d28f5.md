# Luna::memory_profiler_set_memory_domain

```c++
void memory_profiler_set_memory_domain(void *ptr, const c8 *domain, usize str_size=USIZE_MAX)
```

Sets the memory domain. 

The memory domain is usually the heap or pool that allocates this memory block. This function emits one PROFILER_EVENT_ID_SET_MEMORY_DOMAIN profiler event. 

## Parameters
### ptr
The memory block pointer. 

### domain
The domain name for the memory block. 

### str_size
The size of the name, not including the null terminator. If this is `USIZE_MAX`, the size is determined by the system using strlen. 

