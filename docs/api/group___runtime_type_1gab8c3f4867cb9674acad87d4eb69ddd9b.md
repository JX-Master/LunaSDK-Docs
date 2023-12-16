# Luna::is_type_trivially_move_assignable

```c++
bool is_type_trivially_move_assignable(typeinfo_t type)
```

Checks whether one type is a trivially move assignable type. 

One type is trivially move assignable if:1. It is a primitive or enumeration type, or

1. It is a structure or generic structure instanced type without user-provided move assignment function, and all properties of the type are trivially move assignable. 

## Parameters
### type
The type object. 

## Return value
Returns `true` if the specified type is a trivially move assignable type. Returns `false` otherwise. 

## Valid Usage


* `type` must specify one valid type object. 

