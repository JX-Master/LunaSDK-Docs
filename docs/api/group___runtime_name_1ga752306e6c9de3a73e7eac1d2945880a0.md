# Luna::release_name

```c++
void release_name(const c8 *name)
```

Decreases the reference count of the name string by 1, and eventually frees the name string when the reference count goes to 0. 



## Parameters
* *in* **name**

    The pointer of the string. If this is `nullptr`, this call does nothing. 

## Valid Usage
* If `name` is not `nullptr`, it must be a string pointer returned by [intern_name](group___runtime_name_1gaf329effc2cb74e7437566596886907f1.md). 

