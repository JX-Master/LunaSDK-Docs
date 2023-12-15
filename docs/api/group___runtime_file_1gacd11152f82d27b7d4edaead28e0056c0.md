# Luna::move_file

```c++
LUNA_RUNTIME_API RV move_file(const c8 *from_path, const c8 *to_path, FileMoveFlag flags=FileMoveFlag::none)
```

Moves the file or directory from the source path to the destination path. This call can also be used to rename a file. 

## Overview


## Parameters
### from_path
Source file or directory path. 

### to_path
Destination file or directory path. 

### flags
The attributes for one file move operation. 

#### Possible Errors
* BasicError::bad_arguments

* BasicError::already_exists

* BasicError::access_denied

* BasicError::not_found

* BasicError::bad_platform_call for all errors that cannot be identified. 

