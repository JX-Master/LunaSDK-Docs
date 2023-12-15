# Luna::delete_file

```c++
LUNA_RUNTIME_API RV delete_file(const c8 *file_path)
```

Deletes the specified file or directory. 



## Parameters
### file_path
The file or directory to delete. If this is a non-empty directory, all its contexts will also be deleted. 

#### Possible Errors
* BasicError::bad_arguments

* BasicError::not_found

* BasicError::access_denied

* BasicError::bad_platform_call for all errors that cannot be identified. 

