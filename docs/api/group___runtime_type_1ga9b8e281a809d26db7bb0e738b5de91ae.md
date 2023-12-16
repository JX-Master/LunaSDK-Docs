# Luna::hash_type

```c++
usize hash_type(typeinfo_t type, const void *inst)
```

Computes the hash code of one instance of the specified type. 



## Parameters
* *in* **type**

    The type of the instance. 

* *in* **inst**

    The pointer to the instance. 

## Return value
Returns the computed hash code. Returns `0` if the type does not support hash code computing. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type. 

