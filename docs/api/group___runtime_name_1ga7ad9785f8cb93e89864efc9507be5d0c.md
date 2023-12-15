# Luna::retain_name

```c++
LUNA_RUNTIME_API void retain_name(const c8 *name)
```

Increases the reference count of the name string by 1. 

## Overview


## Parameters
### name
The pointer of the string. If this is `nullptr`, this call does nothing. 

#### Valid Usage
* If `name` is not `nullptr`, it must be a string pointer returned by intern_name. 

