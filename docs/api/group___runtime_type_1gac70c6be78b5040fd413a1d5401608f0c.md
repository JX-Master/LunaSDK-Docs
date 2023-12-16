# Luna::copy_construct_type_range

```c++
void copy_construct_type_range(typeinfo_t type, void *dst, void *src, usize count)
```

Copy constructs one array of instances of the specified type. 

The construction is performed as follows:1. If `type` is a trivially copy constructable type, use memcpy to copy instance data.

1. If `type` is a non-trivially-copy-constructable type with user defined copy constructor function, calls the function.

1. If `type` is a non-trivially-copy-constructable type without user defined copy constructor function, copy constructs every property of the structure recursively. 

## Parameters
### type
The type object. 

### dst
The pointer to the instance array to be copy constructed. 

### src
The pointer to the instance array to copy data from. 

### count
The number of instances to construct. 

## Valid Usage


* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

