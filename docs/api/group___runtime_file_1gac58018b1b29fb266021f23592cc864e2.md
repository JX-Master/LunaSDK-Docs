# Luna::open_file

```c++
R< Ref< IFile > > open_file(const c8 *path, FileOpenFlag flags, FileCreationMode creation)
```

Opens one file. 



## Parameters
* *in* **path**

    The path of the file. 

* *in* **flags**

    The file open flags. 

* *in* **creation**

    The file creation mode. 

## Return value
Returns the new opened file object. 

## Possible Errors
* BasicError::bad_arguments

* BasicError::access_denied

* BasicError::not_found

* BasicError::not_directory

* BasicError::bad_platform_call for all errors that cannot be identified. 

