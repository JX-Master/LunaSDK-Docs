# Luna::move_assign_type

```c++
void move_assign_type(typeinfo_t type, void *dst, void *src)
```

Move assigns one instance of the specified type. 

The assignment is performed as follows:1. If `type` is a trivially move assignable type, use memcpy to move instance data.

1. If `type` is a non-trivially-move-assignable type with user defined move assignment function, calls the function.

1. If `type` is a non-trivially-move-assignable type without user defined move assignment function, move assigns every property of the structure recursively. 

## Parameters
* *in* **type**

    The type object. 

* *in* **dst**

    The pointer to the instance to be move assigned. 

* *in* **src**

    The pointer to the instance to move data from. 

## Valid Usage


* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

