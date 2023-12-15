# Luna::object_retain

```c++
LUNA_RUNTIME_API ref_count_t object_retain(object_t object_ptr)
```

Increases the strong refernece counter value by one. 

## Overview


## Parameters
### object_ptr
The object pointer. 

## Return value
Returns the strong reference counter value of the object after the operation. 

#### Valid Usage
* `object_ptr` must points to one memory returned by object_alloc. 

