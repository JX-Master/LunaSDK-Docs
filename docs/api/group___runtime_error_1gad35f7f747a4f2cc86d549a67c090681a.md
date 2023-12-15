# Luna::unwrap_errcode

```c++
template <typename _Ty>
ErrCode unwrap_errcode(const R< _Ty > &obj)
```

Unwraps the real error code from the result. 

If the error code of this result object is `BasicError::error_object`, this function returns the error code stored in the error object of the current thread. If the error code of this object is not `BasicError::error_object`, this function returns the error code as is. 

## Parameters
### obj
The original result object received from the called function. 

## Return value
Returns the real error code from the result. 

