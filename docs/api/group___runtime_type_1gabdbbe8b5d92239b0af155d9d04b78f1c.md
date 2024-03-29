# Luna::register_struct_type

```c++
typeinfo_t register_struct_type(const StructureTypeDesc &desc)
```

Registers one structure type. 

If one type with the same name or GUID already exists, the new type will not be registered. 

## Parameters
* *in* **desc**

    The structure type descriptor. 

## Return value
Returns the type object of the new structure type if the type is successfully registered. Returns the type object of the existing type if one type with the same name or GUID already exists. 

