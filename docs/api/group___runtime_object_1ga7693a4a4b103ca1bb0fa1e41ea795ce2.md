# Luna::get_object_type

```c++
typeinfo_t get_object_type(object_t object_ptr)
```

Gets the type object of the boxed object. 



## Parameters
### object_ptr
The object pointer. 

## Return value
Returns the type object of the boxed object. 

## Valid Usage
* `object_ptr` must points to one memory returned by [object_alloc](group___runtime_object_1ga8ba411b5dc3e81b9d5c0283752e22b9e.md). 

