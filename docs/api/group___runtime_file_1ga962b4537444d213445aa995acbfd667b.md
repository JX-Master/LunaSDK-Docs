# Luna::FileCopyFlag

```c++
enum FileCopyFlag : u32
{
    fail_if_exists= 0x01
}
```

Specify attributes for one file copy operation. 

## Options
* [fail_if_exists](group___runtime_file_1gga962b4537444d213445aa995acbfd667baeec6644eec631f8435646e8695d32403.md)

    If this is specified, the copy operation fails with BasicError::already_exists if the destination file exists. If this is not specified, the destination file will be overwritten by the source file in the copy operation. 

