# Luna::explain

```c++
const c8 * explain(ErrCode err_code)
```

Gets a brief description about the error code. 



## Parameters
* *in* **err_code**

    The error code to fetch. 

## Return value
Returns one C string that describes the error code. 

## Remark
If `err_code` equals to BasicError::error_object, the returned string will be fetched from `get_error().message.c_str(), otherwise, the returned string will be fetched from`get_error_code_name(err_code)`. 

