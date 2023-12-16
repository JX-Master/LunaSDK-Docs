# Luna::construct_type_range

```c++
void construct_type_range(typeinfo_t type, void *data, usize count)
```

Constructs one array of instances of the specified type. 

The construction is performed as follows:1. If `type` is a trivially constructable type, fills the memory with zeros.

1. If `type` is a non-trivially-constructable type with user defined constructor function, calls the function.

1. If `type` is a non-trivially-constructable type without user defined constructor function, constructs every property of the structure recursively. 

## Parameters
* *in* **type**

    The type object. 

* *in* **data**

    The pointer to the instance array. 

* *in* **count**

    The number of instances to construct. 

## Valid Usage


* `type` must specify one valid type object and cannot be a generic structure type.

* `data` must specify one valid memory address. 

