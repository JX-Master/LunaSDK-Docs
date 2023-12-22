# Luna::FileMoveFlag

```c++
enum FileMoveFlag : u32
{
    fail_if_exists= 0x01
}
```

Specify attributes for one file move operation. 

## Options
* [fail_if_exists](group___runtime_file_1gga1c21e7a50d0ce43bee48a939a2b7ab4baeec6644eec631f8435646e8695d32403.md)

    If this is specified, the move operation fails with BasicError::already_exists if the destination file exists. If this is not specified, the destination file will be overwritten by the source file in the move operation. 

