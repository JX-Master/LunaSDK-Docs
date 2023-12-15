# Luna::get_object_type

```c++
LUNA_RUNTIME_API typeinfo_t get_object_type(object_t object_ptr)
```

Gets the type object of the boxed object. 



## Parameters
### object_ptr
The object pointer. 

## Return value
Returns the type object of the boxed object. 

#### Valid Usage
* `object_ptr` must points to one memory returned by object_alloc. 

