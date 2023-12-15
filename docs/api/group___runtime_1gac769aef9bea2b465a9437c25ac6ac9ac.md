# Luna::invoke_r

```c++
template <typename _Return, typename _Func, typename...>
_Return invoke_r(_Func &&f, _Args &&... args)
```

Invokes the specified callable object. 



## Parameters
### f
The callable object to invoke. 

### arg1
The first argument passed to the callable object. 

### args
The rest arguments passed to the callable object. 

## Return value
Returns the return value of the callable object, implicitly converted to `_Return`, if `_Return` is not void. None otherwise. 

