# Luna::is_type_trivially_constructable

```c++
bool is_type_trivially_constructable(typeinfo_t type)
```

Checks whether one type is a trivially constructable type. 

One type is trivially constructable if:1. It is a primitive or enumeration type, or

1. It is a structure or generic structure instanced type without user-provided constructor function, and all properties of the type are trivially constructable. 

## Parameters
* *in* **type**

    The type object. 

## Return value
Returns `true` if the specified type is a trivially constructable type. Returns `false` otherwise. 

## Valid Usage


* `type` must specify one valid type object. 

