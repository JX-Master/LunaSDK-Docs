# Luna::object_expired

```c++
LUNA_RUNTIME_API bool object_expired(object_t object_ptr)
```

Checks if the boxed object is expired, that is, destructed but its memeory is not freed. 

One object will be expired if its strong reference counter value drops 0, but its weak reference counter value is not 0. 

## Parameters
### object_ptr
The object pointer. 

## Return value
Returns `true` if the object is expired, returns `false` otherwise. 

#### Valid Usage
* `object_ptr` must points to one memory returned by object_alloc. 

