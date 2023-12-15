# Luna::allocate_profiler_event_data

```c++
LUNA_RUNTIME_API void * allocate_profiler_event_data(usize size, usize alignment, void(*dtor)(void *)=nullptr)
```

Allocates one temporary buffer that can be used to store event data for the next profiler event. 

## Overview


## Parameters
### size
The size to allocate in bytes. 

### alignment
The alignment requirement of the allocated memory in bytes. This can be `0`, indicating that no alignment requirement is specified. 

### dtor
The function that will be called when the memory is going to be freed. This can be `nullptr`, indicating that no operation is performed before freeing memory. 

## Return value
Returns the allocated memory. 

#### Valid Usage
* If `alignment` is not `0`, `alignment` must be power of 2 (like 4, 8, 16, etc.). 

