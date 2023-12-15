# Luna::object_retain_if_not_expired

```c++
LUNA_RUNTIME_API bool object_retain_if_not_expired(object_t object_ptr)
```

Increases the strong refernece counter value by one if the boxed object is not expired. 

## Overview
This call is atomic and can be used to create strong references from weak references. 

## Parameters
### object_ptr
The object pointer. 

## Return value
Returns `true` if the object is valid and the strong reference counter value is successfully increased, returns `false` otherwise. 

#### Valid Usage
* `object_ptr` must points to one memory returned by object_alloc. 

