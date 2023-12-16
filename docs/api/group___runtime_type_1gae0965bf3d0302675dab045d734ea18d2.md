# Luna::is_type_trivially_relocatable

```c++
bool is_type_trivially_relocatable(typeinfo_t type)
```

Checks whether one type is a trivially relocatable type. 

One type is trivially relocatable if:1. It is a primitive or enumeration type, or

1. It is a structure or generic structure instanced type with `trivially_relocatable` set to `true`. 

## Parameters
* *in* **type**

    The type object. 

## Return value
Returns `true` if the specified type is a trivially relocatable type. Returns `false` otherwise. 

## Valid Usage


* `type` must specify one valid type object. 

