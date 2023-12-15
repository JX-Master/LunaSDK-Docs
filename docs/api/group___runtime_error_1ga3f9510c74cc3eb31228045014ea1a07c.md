# Luna::unwrap_errcode

```c++
ErrCode unwrap_errcode(ErrCode err_code)
```

Gets the real error code if the error code is BasicError::error_object. 



## Parameters
### err_code
The error code to unwrap. 

## Return value
If the error code is BasicError::error_object, returns `get_error().code`. Otherwise, returns `err_code` directly. 

