# Luna::object_release_weak

```c++
ref_count_t object_release_weak(object_t object_ptr)
```

Decreases the weak refernece counter value by one. 



## Parameters
* *in* **object_ptr**

    The object pointer. 

## Return value
Returns the weak reference counter value of the object after the operation. 

## Valid Usage
* `object_ptr` must points to one memory returned by [object_alloc](group___runtime_object_1gabbcaac45f20e9e4c322fb1db0376b641.md). 

