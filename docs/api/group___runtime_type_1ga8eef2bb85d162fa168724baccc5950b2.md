# Luna::set_type_private_data

```c++
LUNA_RUNTIME_API void * set_type_private_data(typeinfo_t type, const Guid &data_guid, usize data_size, usize data_alignment=0, void(*data_dtor)(void *)=nullptr)
```

Sets user defined private data for the specified type. 



## Parameters
### type
The type object. 

### data_guid
The GUID of the private data. If one data with this GUID already exists, the original data will be deleted and replaced by one new data. 

### data_size
The size of the data in bytes. 

### data_alignment
The alignment requirement of the data in bytes. Specify `0` to use the default alignment, which is MAX_ALIGN. 

### data_dtor
One optional callback function that will be called when the data is going to be freed if specified. 

#### Valid Usage
* `type` must specify one valid type object. 

