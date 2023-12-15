# Luna::object_is_type

```c++
LUNA_RUNTIME_API bool object_is_type(object_t object_ptr, typeinfo_t type)
```

Checks whether the boxed object is the specified type or derived types of the specified type. 



## Parameters
### object_ptr
The object pointer. 

## Return value
Returns `true` if the boxed object is the specified type or derived types of the specified type, returns `false` otherwise. 

#### Valid Usage
* `object_ptr` must points to one memory returned by object_alloc. 

