# Luna::object_release

```c++
LUNA_RUNTIME_API ref_count_t object_release(object_t object_ptr)
```

Decreases the strong refernece counter value by one, and destroys the object if the reference counter drops to 0. 

## Overview


## Parameters
### object_ptr
The object pointer. 

## Return value
Returns the strong reference counter value of the object after the operation. 

#### Valid Usage
* `object_ptr` must points to one memory returned by object_alloc. 

