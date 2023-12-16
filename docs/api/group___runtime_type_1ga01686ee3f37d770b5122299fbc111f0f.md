# Luna::is_type_trivially_destructable

```c++
bool is_type_trivially_destructable(typeinfo_t type)
```

Checks whether one type is a trivially destructable type. 

One type is trivially destructable if:1. It is a primitive or enumeration type, or

1. It is a structure or generic structure instanced type without user-provided destructor function, and all properties of the type are trivially destructable. 

## Parameters
* *in* **type**

    The type object. 

## Return value
Returns `true` if the specified type is a trivially destructable type. Returns `false` otherwise. 

## Valid Usage


* `type` must specify one valid type object. 

