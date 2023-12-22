# Luna::memory_profiler_set_memory_type

```c++
void memory_profiler_set_memory_type(void *ptr, const c8 *type, usize str_size=USIZE_MAX)
```

Sets the type of the object this memory block. 



## Parameters
* *in* **ptr**

    The memory block pointer. 

* *in* **domain**

    The type name for the memory block. 

* *in* **str_size**

    The size of the name, not including the null terminator. If this is `USIZE_MAX`, the size is determined by the system using [strlen](group___runtime_string_1gacabe981ca12e2bfa89fc57ca022360a5.md). 

