# Luna::create_dir

```c++
RV create_dir(const c8 *path)
```

Creates one empty directory. 



## Parameters
* *in* **path**

    The path of the directory to create. 

## Possible Errors
* BasicError::already_exists

* BasicError::not_found

* BasicError::bad_platform_call for all errors that cannot be identified. 

