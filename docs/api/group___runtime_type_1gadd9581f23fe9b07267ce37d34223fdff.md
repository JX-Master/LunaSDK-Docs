# Luna::is_type_equatable

```c++
bool is_type_equatable(typeinfo_t type)
```

Checks whether the specified type supports equality testing. 



## Parameters
* *in* **type**

    The type object. 

## Return value
Returns `true` if the specified type supports equality testing. Returns `false` otherwise. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type. 

