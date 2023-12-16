# Luna::move_assign_type_range

```c++
void move_assign_type_range(typeinfo_t type, void *dst, void *src, usize count)
```

Move assigns one array of instances of the specified type. 

The assignment is performed as follows:1. If `type` is a trivially move assignable type, use memcpy to move instance data.

1. If `type` is a non-trivially-move-assignable type with user defined move assignment function, calls the function.

1. If `type` is a non-trivially-move-assignable type without user defined move assignment function, move assigns every property of the structure recursively. 

## Parameters
### type
The type object. 

### dst
The pointer to the instance array to be move assigned. 

### src
The pointer to the instance array to move data from. 

### count
The number of instances to assign. 

## Valid Usage


* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

