# Luna::destruct_type

```c++
void destruct_type(typeinfo_t type, void *data)
```

Destructs one instance of the specified type. 

The destruction is performed as follows:1. If `type` is a trivially destructable type, does nothing.

1. If `type` is a non-trivially-destructable type with user defined destructor function, calls the function.

1. If `type` is a non-trivially-destructable type without user defined destructor function, destructs every property of the structure recursively. 

## Parameters
* *in* **type**

    The type object. 

* *in* **data**

    The pointer to the instance. 

## Valid Usage


* `type` must specify one valid type object and cannot be a generic structure type.

* `data` must specify one valid memory address. 

