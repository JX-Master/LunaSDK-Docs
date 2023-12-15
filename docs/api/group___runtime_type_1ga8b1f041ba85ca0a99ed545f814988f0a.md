# Luna::get_type_private_data

```c++
LUNA_RUNTIME_API void * get_type_private_data(typeinfo_t type, const Guid &data_guid)
```

Gets user defined private data for the specified type. 



## Parameters
### type
The type object. 

### data_guid
The GUID of the private data to check. 

## Return value
Returns one pointer to the private data. Returns `nullptr` if such data does not exist. 

#### Valid Usage
* `type` must specify one valid type object. 

