# Luna::object_ref_count

```c++
LUNA_RUNTIME_API ref_count_t object_ref_count(object_t object_ptr)
```

Fetches the strong refernece counter value of the boxed object. 



## Parameters
### object_ptr
The object pointer. 

## Return value
Returns the strong reference counter value of the object. 

#### Valid Usage
* `object_ptr` must points to one memory returned by object_alloc. 

