# Luna::allocate_profiler_event_data

```c++
template <typename _Ty>
_Ty * allocate_profiler_event_data()
```

Allocates one temporary object that can be used to store event data for the next profiler event. 

This function uses the specified type to provide size, alignment and destructor for the memory. 

## Return value
Returns the allocated object. The returned object is not initialized, the user should call `new (ptr) _Ty(...)` to initialize the object manually. 

