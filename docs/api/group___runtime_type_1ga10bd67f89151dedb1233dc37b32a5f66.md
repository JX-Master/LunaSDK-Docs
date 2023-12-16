# Luna::equal_to_type

```c++
bool equal_to_type(typeinfo_t type, const void *lhs, const void *rhs)
```

Checks whether two instances of one type are equal. 



## Parameters
### type
The type object. 

### lhs
The pointer to the first instance to be compared. 

### rhs
The pointer to the second instance to be compared. 

## Return value
Returns `true` if two instances are equal. Returns `false` otherwise. Returns `false` if the type does not support equality testing. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type. 

