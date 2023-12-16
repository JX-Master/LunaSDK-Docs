# Luna::set_error

```c++
ErrCode set_error(ErrCode code, const c8 *fmt, VarList args)
```

Sets the error object of this thread. 

This function is auxiliary and it behaves the same as fetching the error object then setting it. 

## Parameters
* *in* **code**

    The error code to set. 

* *in* **fmt**

    The error message formatting syntax. 

* *in* **args**

    The arguments for the error message. 

## Return value
Returns BasicError::error_object always, so you may chain this function with the return statement like `return set_error(...)`. 

