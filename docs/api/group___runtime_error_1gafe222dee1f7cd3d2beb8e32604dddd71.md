# Luna::get_error_category_by_name

```c++
LUNA_RUNTIME_API errcat_t get_error_category_by_name(const c8 *errcat_name)
```

Gets the error category represented by the error category name. 



## Parameters
### errcat_name
The full name of the error category. Use "::" to separate category names if the category is a sub-category. 

## Return value
Returns the error category of the corresponding error name. The return value will never be 0, if the error category name is required for the first time, the system creates one new registry for the error category, and returns one valid error category number that represents to the error category. 

