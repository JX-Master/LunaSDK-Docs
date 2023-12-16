# Luna::relocate_type

```c++
void relocate_type(typeinfo_t type, void *dst, void *src)
```

Relocates one instance of the specified type. 

The relocation is performed as follows:1. If `type` is a trivially relocatable type, use memcpy to move instance data.

1. If `type` is a non-trivially-relocatable type, use [move_construct_type](group___runtime_type_1gac7867a132f5246297db7b59105df8f9b.md) to move construct one new instance on new location, then use [destruct_type](group___runtime_type_1gaf8ad2e47bfbc89371f6d2ef227c39f28.md) to destruct the old instance. 

## Parameters
* *in* **type**

    The type object. 

* *in* **dst**

    The pointer to the instance to be relocated. 

* *in* **src**

    The pointer to the new location of the instance. 

