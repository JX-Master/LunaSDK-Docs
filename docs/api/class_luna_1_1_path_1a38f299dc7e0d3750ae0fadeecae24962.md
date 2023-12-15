# Luna::Path::assign_relative

```c++
void assign_relative(const Path &base, const Path &target)
```

Assigns the content of this path with a new path that if appended to `base` path, creates a path equal to `target` path. 

## Overview


## Parameters
### base
The base path. 

### target
The target path. 

## Return value
If the system can decide how to redirect target path to this path, returns the relative path, else, returns failure. 

