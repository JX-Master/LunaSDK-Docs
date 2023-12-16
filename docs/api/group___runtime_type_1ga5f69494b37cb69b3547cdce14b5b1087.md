# Luna::copy_construct_type

```c++
void copy_construct_type(typeinfo_t type, void *dst, void *src)
```

Copy constructs one instance of the specified type. 

The construction is performed as follows:1. If `type` is a trivially copy constructable type, use memcpy to copy instance data.

1. If `type` is a non-trivially-copy-constructable type with user defined copy constructor function, calls the function.

1. If `type` is a non-trivially-copy-constructable type without user defined copy constructor function, copy constructs every property of the structure recursively. 

## Parameters
* *in* **type**

    The type object. 

* *in* **dst**

    The pointer to the instance to be copy constructed. 

* *in* **src**

    The pointer to the instance to copy data from. 

## Valid Usage


* `type` must specify one valid type object and cannot be a generic structure type.

* `dst` and `src` must specify one valid memory address. 

