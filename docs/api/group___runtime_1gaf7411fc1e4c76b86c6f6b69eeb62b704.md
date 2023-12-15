# Luna::invoke

```c++
template <typename _Func>
auto invoke(_Func &&f) -> decltype(static_cast< _Func && >(f)())
```

Invokes the specified callable object. 



## Parameters
### f
The callable object to invoke. 

## Return value
Returns the return value of the callable object. 

