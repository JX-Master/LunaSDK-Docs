# Luna::get_file_attribute

```c++
R< FileAttribute > get_file_attribute(const c8 *path)
```

Gets the file attribute. 



## Parameters
### path
The path of the file. 

## Return value
Returns the file attribute structure. 

## Possible Errors
* BasicError::access_denied

* BasicError::not_found

* BasicError::not_directory

* BasicError::bad_platform_call for all errors that cannot be identified. 

