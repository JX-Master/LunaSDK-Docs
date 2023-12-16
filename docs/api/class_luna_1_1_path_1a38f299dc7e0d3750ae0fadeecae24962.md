# Luna::Path::assign_relative

```c++
void assign_relative(const Path &base, const Path &target)
```

Assigns the content of this path with a new path that if appended to `base` path, creates a path equal to `target` path. 



## Parameters
* *in* **base**

    The base path. 

* *in* **target**

    The target path. 

## Return value
If the system can decide how to redirect target path to this path, returns the relative path, else, returns failure. 

## Remark
In order to let this function succeeds, the following conditions are required:1. The root name of this path and target path must be equal, either `nullptr` or points to the same `Name` object.

1. Both path should either all be absolute or all be relative. The returned path has the same root name as this path, and will always be a relative path. If this path is a directory, then the returned path will be marked as directory. The target path will always be recognized as directory, no matter if it is marked as directory. 

