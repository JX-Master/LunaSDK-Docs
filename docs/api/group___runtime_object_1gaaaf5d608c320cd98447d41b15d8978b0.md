# Luna::get_object_type

```c++
typeinfo_t get_object_type(object_t object_ptr)
```

Gets the type object of the boxed object. 



## Parameters
* *in* **object_ptr**

    The object pointer. 

## Return value
Returns the type object of the boxed object. 

## Valid Usage
* `object_ptr` must points to one memory returned by [object_alloc](group___runtime_object_1gabbcaac45f20e9e4c322fb1db0376b641.md). 

