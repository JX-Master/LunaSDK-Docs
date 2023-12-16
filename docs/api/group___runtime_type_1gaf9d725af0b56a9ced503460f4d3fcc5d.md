# Luna::get_struct_properties

```c++
Span< const StructurePropertyDesc > get_struct_properties(typeinfo_t type)
```

Gets properties of the specified structure. 



## Parameters
### type
The type to query. 

## Return value
Returns properties of the specified structure. The returned buffer is valid until SDK shutdown. Returns one empty range if `type` is not a structure or generic structure instanced type. 

## Valid Usage
* `type` must specify one valid type object. 

