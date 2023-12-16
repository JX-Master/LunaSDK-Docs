# Luna::object_release

```c++
ref_count_t object_release(object_t object_ptr)
```

Decreases the strong refernece counter value by one, and destroys the object if the reference counter drops to 0. 



## Parameters
### object_ptr
The object pointer. 

## Return value
Returns the strong reference counter value of the object after the operation. 

## Valid Usage
* `object_ptr` must points to one memory returned by [object_alloc](group___runtime_object_1ga8ba411b5dc3e81b9d5c0283752e22b9e.md). 

