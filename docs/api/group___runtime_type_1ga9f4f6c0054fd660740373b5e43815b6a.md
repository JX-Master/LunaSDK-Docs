# Luna::get_type_private_data

```c++
void * get_type_private_data(typeinfo_t type, const Guid &data_guid)
```

Gets user defined private data for the specified type. 



## Parameters
* *in* **type**

    The type object. 

* *in* **data_guid**

    The GUID of the private data to check. 

## Return value
Returns one pointer to the private data. Returns `nullptr` if such data does not exist. 

## Valid Usage
* `type` must specify one valid type object. 

