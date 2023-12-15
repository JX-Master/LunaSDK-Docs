# Luna::memory_profiler_allocate

```c++
LUNA_RUNTIME_API void memory_profiler_allocate(void *ptr, usize size)
```

Emits one PROFILER_EVENT_ID_MEMORY_ALLOCATE profiler event. 



## Parameters
### ptr
The pointer that represents the memory. This pointer is used only for identifing the memory block, it may not be the real memory address of the memory block, but must be unique in the application domain. 

### size
The size of the memory block, in bytes. 

