# Luna::object_retain

```c++
ref_count_t object_retain(object_t object_ptr)
```

Increases the strong refernece counter value by one. 



## Parameters
* *in* **object_ptr**

    The object pointer. 

## Return value
Returns the strong reference counter value of the object after the operation. 

## Valid Usage
* `object_ptr` must points to one memory returned by [object_alloc](group___runtime_object_1gabbcaac45f20e9e4c322fb1db0376b641.md). 

