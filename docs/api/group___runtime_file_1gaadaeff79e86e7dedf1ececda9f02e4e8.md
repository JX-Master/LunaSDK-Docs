# Luna::copy_file

```c++
RV copy_file(const c8 *from_path, const c8 *to_path, FileCopyFlag flags=FileCopyFlag::none)
```

Copies the file or directory from the source path to the destination path. 



## Parameters
* *in* **from_path**

    Source file or directory path. 

* *in* **to_path**

    Destination file or directory path. 

* *in* **flags**

    The attributes for one file copy operation. 

## Possible Errors
* BasicError::bad_arguments

* BasicError::already_exists

* BasicError::access_denied

* BasicError::not_found

* BasicError::bad_platform_call for all errors that cannot be identified. 

