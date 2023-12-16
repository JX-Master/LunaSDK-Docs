# Luna::register_profiler_callback

```c++
usize register_profiler_callback(const Function< on_profiler_event_t > &handler)
```

Registers one profiler callback function. 



## Parameters
* *in* **handler**

    The callback function object to register. 

## Return value
Returns one handle that can be used to unregister the callback function. 

