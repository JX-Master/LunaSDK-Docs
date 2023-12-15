# Luna::set_error

```c++
ErrCode set_error(ErrCode code, const c8 *fmt, VarList args)
```

Sets the error object of this thread. 

## Overview
This function is auxiliary and it behaves the same as fetching the error object then setting it. 

## Parameters
### code
The error code to set. 

### fmt
The error message formatting syntax. 

### args
The arguments for the error message. 

## Return value
Returns BasicError::error_object always, so you may chain this function with the return statement like `return set_error(...)`. 

