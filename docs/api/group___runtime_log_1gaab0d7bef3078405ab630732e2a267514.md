# Luna::logv_debug

```c++
LUNA_RUNTIME_API void logv_debug(const c8 *tag, const c8 *format, VarList args)
```

Outputs one log message with LogVerbosity::debug verbosity. 

## Overview


## Parameters
### tag
The log tag. Used by the implementation to filter logs. 

### format
The formatting syntax used to format the log message. 

### args
Arguments used to format the log message. 
