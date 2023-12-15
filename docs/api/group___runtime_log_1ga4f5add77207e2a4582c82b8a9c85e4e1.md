# Luna::log_callback_t

```c++
using log_callback_t =  void(LogVerbosity verbosity, const c8* tag, usize tag_length, const c8* message, usize message_length)
```

Called by the log system when one log is emitted. 

## Overview


## Parameters
### verbosity
The log verbosity. 

### tag
The log tag. Used by the implementation to filter logs. 

### tag_len
The length of the tag string. 

### message
The log message. 

### message_length
The message length. 

