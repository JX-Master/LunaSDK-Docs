# Luna::hash_type

```c++
LUNA_RUNTIME_API usize hash_type(typeinfo_t type, const void *inst)
```

Computes the hash code of one instance of the specified type. 



## Parameters
### type
The type of the instance. 

### inst
The pointer to the instance. 

## Return value
Returns the computed hash code. Returns `0` if the type does not support hash code computing. 

#### Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type. 

