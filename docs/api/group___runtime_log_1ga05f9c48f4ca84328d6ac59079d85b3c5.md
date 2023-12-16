# Luna::flush_log_to_file

```c++
void flush_log_to_file()
```

Flushes the log-to-file cache and writes all cached logs to the log file. 



## Remark
For performance reasons, when logging-to-file is enabled, log messages will be cached in a log buffer and written to the log file in one call when the buffer is full. The user can also call [flush_log_to_file](group___runtime_log_1ga05f9c48f4ca84328d6ac59079d85b3c5.md) to flush the cache manually when needed. 

