# Luna::move_construct_type_range

```c++
void move_construct_type_range(typeinfo_t type, void *dst, void *src, usize count)
```

Move constructs one array of instances of the specified type. 

The construction is performed as follows:1. If `type` is a trivially move constructable type, use memcpy to move instance data.

1. If `type` is a non-trivially-move-constructable type with user defined move constructor function, calls the function.

1. If `type` is a non-trivially-move-constructable type without user defined move constructor function, move constructs every property of the structure recursively. 

## Parameters
* *in* **type**

    The type object. 

* *in* **dst**

    The pointer to the instance array to be move constructed. 

* *in* **src**

    The pointer to the instance array to move data from. 

* *in* **count**

    The number of instances to construct. 

## Valid Usage


* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

