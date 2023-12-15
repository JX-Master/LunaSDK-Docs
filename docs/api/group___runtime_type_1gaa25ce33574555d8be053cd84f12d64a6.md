# Luna::equal_to_func_t

```c++
using equal_to_func_t =  bool(typeinfo_t type, const void* lhs, const void* rhs)
```

The equality testing function used by the reflection system. 



## Parameters
### type
The type object. 

### lhs
The pointer to the first instance to be compared. 

### rhs
The pointer to the second instance to be compared. 

## Return value
Returns `true` if two instances are equal. Returns `false` otherwise. 

