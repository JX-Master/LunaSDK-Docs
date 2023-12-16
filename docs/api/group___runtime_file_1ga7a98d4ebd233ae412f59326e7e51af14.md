# Luna::open_dir

```c++
R< Ref< IFileIterator > > open_dir(const c8 *path)
```

Creates a file iterator that can be used to iterate all files in the specified directory. 



## Parameters
* *in* **path**

    The directory path to open. 

## Return value
Returns a file iterator object. 

## Possible Errors
* BasicError::not_found

* BasicError::bad_platform_call for all errors that cannot be identified. 

