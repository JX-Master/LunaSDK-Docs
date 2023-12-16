# Luna::set_hashable

```c++
void set_hashable(typeinfo_t type, hash_func_t *func)
```

Sets one type to support hash code computing. 



## Parameters
### type
The type object. 

### func
The hash code computing function to use. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type.

* `func` must specify one valid function. 

