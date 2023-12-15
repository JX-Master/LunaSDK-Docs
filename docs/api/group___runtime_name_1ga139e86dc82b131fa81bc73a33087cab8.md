# Luna::get_name_size

```c++
LUNA_RUNTIME_API usize get_name_size(const c8 *name)
```

Fetches the size of the name string. 



## Parameters
### name
The pointer of the string. 

## Return value
Returns the size of the name. Returns `0` if `name` is `nullptr`. 


The size of the name is cached in the system, so this call returns in constant time. 

#### Valid Usage
* If `name` is not `nullptr`, it must be a string pointer returned by intern_name. 

