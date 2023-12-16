# Luna::object_retain_weak

```c++
ref_count_t object_retain_weak(object_t object_ptr)
```

Increases the weak refernece counter value by one. 



## Parameters
### object_ptr
The object pointer. 

## Return value
Returns the weak reference counter value of the object after the operation. 

## Valid Usage
* `object_ptr` must points to one memory returned by [object_alloc](group___runtime_object_1ga8ba411b5dc3e81b9d5c0283752e22b9e.md). 

