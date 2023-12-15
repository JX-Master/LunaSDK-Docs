# Luna::get_type_by_guid

```c++
LUNA_RUNTIME_API typeinfo_t get_type_by_guid(const Guid &guid)
```

Gets the type object from one type GUID. 

## Overview


## Parameters
### guid
The GUID of the type. 

## Return value
Returns the type object for the GUID. Returns `nullptr` if the specified type is not found. 

