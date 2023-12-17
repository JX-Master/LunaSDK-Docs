# Luna::FileMoveFlag::fail_if_exists

```c++
fail_if_exists = 0x01
```

If this is specified, the move operation fails with BasicError::already_exists if the destination file exists. If this is not specified, the destination file will be overwritten by the source file in the move operation. 

