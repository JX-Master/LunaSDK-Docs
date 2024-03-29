# Luna::invoke

```c++
template <typename _Func, typename _Ty, typename...>
auto invoke(_Func &&f, _Ty &&arg1, _Args &&... args) -> invoke_result_t< _Func, _Ty, _Args... >
```

Invokes the specified callable object. 



## Parameters
* *in* **f**

    The callable object to invoke. 

* *in* **arg1**

    The first argument passed to the callable object. 

* *in* **args**

    The rest arguments passed to the callable object. 

## Return value
Returns the return value of the callable object. 

