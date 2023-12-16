# Luna::set_type_private_data

```c++
void * set_type_private_data(typeinfo_t type, const Guid &data_guid, usize data_size, usize data_alignment=0, void(*data_dtor)(void *)=nullptr)
```

Sets user defined private data for the specified type. 



## Parameters
* *in* **type**

    The type object. 

* *in* **data_guid**

    The GUID of the private data. If one data with this GUID already exists, the original data will be deleted and replaced by one new data. 

* *in* **data_size**

    The size of the data in bytes. 

* *in* **data_alignment**

    The alignment requirement of the data in bytes. Specify `0` to use the default alignment, which is [MAX_ALIGN](group___runtime_base_type_1gae771c7d05b7f7738144b784fa44ce6a9.md). 

* *in* **data_dtor**

    One optional callback function that will be called when the data is going to be freed if specified. 

## Valid Usage
* `type` must specify one valid type object. 

