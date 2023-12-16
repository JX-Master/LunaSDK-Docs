# Luna::log_callback_t

```c++
using log_callback_t =  void(LogVerbosity verbosity, const c8* tag, usize tag_length, const c8* message, usize message_length)
```

Called by the log system when one log is emitted. 



## Parameters
* *in* **verbosity**

    The log verbosity. 

* *in* **tag**

    The log tag. Used by the implementation to filter logs. 

* *in* **tag_len**

    The length of the tag string. 

* *in* **message**

    The log message. 

* *in* **message_length**

    The message length. 

