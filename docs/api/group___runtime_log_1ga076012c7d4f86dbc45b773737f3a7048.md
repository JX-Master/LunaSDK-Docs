# Luna::register_log_handler

```c++
usize register_log_handler(const Function< log_callback_t > &handler)
```

Registers one custom log handler that will be called when a new log message is spawned. 



## Parameters
* *in* **handler**

    The handler to register. 

## Return value
Returns one handler identifier that can be used to register the handler. 

