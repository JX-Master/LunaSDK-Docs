# Luna::VFS::delete_file

```c++
RV delete_file(const Path &path)
```

Deletes the specified file. 



## Parameters
* *in* **path**

    The file to delete. 

## Possible Errors:
* BasicError::bad_arguments

* BasicError::not_found

* BasicError::access_denied

* BasicError::bad_platform_call for all errors that cannot be identified. 

