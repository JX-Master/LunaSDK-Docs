# Luna::copy_assign_type_range

```c++
void copy_assign_type_range(typeinfo_t type, void *dst, void *src, usize count)
```

Copy assigns one array of instances of the specified type. 

The assignment is performed as follows:1. If `type` is a trivially copy assignable type, use memcpy to copy instance data.

1. If `type` is a non-trivially-copy-assignable type with user defined copy assignment function, calls the function.

1. If `type` is a non-trivially-copy-assignable type without user defined copy assignment function, copy assigns every property of the structure recursively. 

## Parameters
* *in* **type**

    The type object. 

* *in* **dst**

    The pointer to the instance array to be copy assigned. 

* *in* **src**

    The pointer to the instance array to copy data from. 

* *in* **count**

    The number of instances to assign. 

## Valid Usage


* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

