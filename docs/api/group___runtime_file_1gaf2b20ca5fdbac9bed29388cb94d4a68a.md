# Luna::get_current_dir

```c++
u32 get_current_dir(u32 buffer_length, c8 *buffer)
```

Gets the current working directory path for the underlying system. 

The default current working directory is set to the path that contains the executable file. 

## Parameters
### buffer_length
The length of the buffer for the current directory string, including the null terminator. 

### buffer
A pointer to the buffer that receives the current directory string. To gets the required buffer size, specify buffer to `nullptr` and buffer_length to 0. 

## Return value
Returns the number of characters copied into the buffer, including the null terminator. The copied string is always null-terminated. If buffer_length is `0` and buffer is `nullptr`, returns the required buffer size to fetch the current directory, including the null terminator. 

