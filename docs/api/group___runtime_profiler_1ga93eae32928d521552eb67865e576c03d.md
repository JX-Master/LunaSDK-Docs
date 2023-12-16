# Luna::memory_profiler_allocate

```c++
void memory_profiler_allocate(void *ptr, usize size)
```

Emits one PROFILER_EVENT_ID_MEMORY_ALLOCATE profiler event. 



## Parameters
* *in* **ptr**

    The pointer that represents the memory. This pointer is used only for identifing the memory block, it may not be the real memory address of the memory block, but must be unique in the application domain. 

* *in* **size**

    The size of the memory block, in bytes. 

## Remark
Memory allocations through `memalloc` call this internally when memory profiling is enabled, thus the user does not need to call this again. 

