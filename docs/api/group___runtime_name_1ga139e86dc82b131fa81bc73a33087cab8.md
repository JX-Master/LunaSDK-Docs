# Luna::get_name_size

```c++
usize get_name_size(const c8 *name)
```

Fetches the size of the name string. 



## Parameters
### name
The pointer of the string. 

## Return value
Returns the size of the name. Returns `0` if `name` is `nullptr`. 

## Remark
Note that the size returned is not always equal to the size returnd by `strlen`, since the string that contains the null terminator is allowed as a name, so always fetches the name size using this API.


The size of the name is cached in the system, so this call returns in constant time. 

## Valid Usage
* If `name` is not `nullptr`, it must be a string pointer returned by [intern_name](group___runtime_name_1gaa261ca6305ee4dee587492a004d6f9ee.md). 

