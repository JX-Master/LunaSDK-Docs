# Luna::get_error_category_name

```c++
LUNA_RUNTIME_API const c8 * get_error_category_name(errcat_t err_category)
```

Fetches the name of the error category. 



## Parameters
### err_category
The error category value. 

## Return value
Returns the name of the error category. This string is valid until the runtime is closed. Returns empty string ("") if the error category does not exist. 

