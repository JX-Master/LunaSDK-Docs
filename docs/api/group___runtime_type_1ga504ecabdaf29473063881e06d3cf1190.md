# Luna::is_type_hashable

```c++
bool is_type_hashable(typeinfo_t type)
```

Checks whether the specified type supports hash code computing. 



## Parameters
* *in* **type**

    The type object. 

## Return value
Returns `true` if the specified type supports hash code computing. Returns `false` otherwise. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type. 

