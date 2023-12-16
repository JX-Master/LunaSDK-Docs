# Luna::set_log_file

```c++
void set_log_file(const c8 *file)
```

Sets the file path of the log file. 



## Parameters
* *in* **file**

    The file path of the log file. The file path may be absolute or relative to the current working directory. 

## Remark
If the log file path is not set by the user, the default log file path will be `"./Log.txt"`. 

