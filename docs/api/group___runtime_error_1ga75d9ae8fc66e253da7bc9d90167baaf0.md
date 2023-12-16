# Luna::get_error_code_name

```c++
const c8 * get_error_code_name(ErrCode err_code)
```

Fetches the name of the error code. 



## Parameters
* *in* **err_code**

    The error code value. 

## Return value
Returns the name of the error code. This string is valid until the runtime is closed. Returns empty string ("") if the error code does not exist. 

