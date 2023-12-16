# Luna::is_type_trivially_copy_constructable

```c++
bool is_type_trivially_copy_constructable(typeinfo_t type)
```

Checks whether one type is a trivially copy constructable type. 

One type is trivially copy constructable if:1. It is a primitive or enumeration type, or

1. It is a structure or generic structure instanced type without user-provided copy constructor function, and all properties of the type are trivially copy constructable. 

## Parameters
* *in* **type**

    The type object. 

## Return value
Returns `true` if the specified type is a trivially copy constructable type. Returns `false` otherwise. 

## Valid Usage


* `type` must specify one valid type object. 

