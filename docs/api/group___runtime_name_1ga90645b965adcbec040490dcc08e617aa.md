# Luna::get_name_id

```c++
LUNA_RUNTIME_API name_id_t get_name_id(const c8 *name)
```

Gets the ID for the specified name. The ID keeps constant between multiple processes. 

Since the name ID is hashed from the name string, technically multiple names may have the same ID. The name system handles such confliction, so that different name string will always have different pointer, even they have the same ID. The user should compare the string pointer returned by intern_name rather than the string ID to check whether two strings are equal. 

## Parameters
### name
The pointer of the string. If this is `nullptr`, this call returns `0`. 

#### Valid Usage
* If `name` is not `nullptr`, it must be a string pointer returned by intern_name. 

