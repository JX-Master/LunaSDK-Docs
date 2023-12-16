# Luna::get_error_code_by_name

```c++
ErrCode get_error_code_by_name(const c8 *errcat_name, const c8 *errcode_name)
```

Gets the error code represented by the error name. 



## Parameters
* *in* **errcat_name**

    The name of the category that holds the error name. Use "::" to separate category names if the category is a sub-category. 

* *in* **errcode_name**

    The name of the error code. 

## Return value
Returns the error code of the corresponding error name. The return value will never be 0, if the error code name is required for the first time, the system creates one new registry for the error code, and returns one valid error code number that represents to the error. 

