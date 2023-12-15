# Luna::object_release_weak

```c++
LUNA_RUNTIME_API ref_count_t object_release_weak(object_t object_ptr)
```

Decreases the weak refernece counter value by one. 



## Parameters
### object_ptr
The object pointer. 

## Return value
Returns the weak reference counter value of the object after the operation. 

#### Valid Usage
* `object_ptr` must points to one memory returned by object_alloc. 

