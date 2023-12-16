# Luna::copy_assign_type

```c++
void copy_assign_type(typeinfo_t type, void *dst, void *src)
```

Copy assigns one instance of the specified type. 

The assignment is performed as follows:1. If `type` is a trivially copy assignable type, use memcpy to copy instance data.

1. If `type` is a non-trivially-copy-assignable type with user defined copy assignment function, calls the function.

1. If `type` is a non-trivially-copy-assignable type without user defined copy assignment function, copy assigns every property of the structure recursively. 

## Parameters
### type
The type object. 

### dst
The pointer to the instance to be copy assigned. 

### src
The pointer to the instance to copy data from. 

## Valid Usage


* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

