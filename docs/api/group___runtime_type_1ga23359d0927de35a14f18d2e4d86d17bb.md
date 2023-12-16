# Luna::register_enum_type

```c++
typeinfo_t register_enum_type(const EnumerationTypeDesc &desc)
```

Registers one enumeration type. 

If one type with the same name or GUID already exists, the new type will not be registered. 

## Parameters
* *in* **desc**

    The enumeration type descriptor. 

## Return value
Returns the type object of the new enumeration type if the type is successfully registered. Returns the type object of the existing type if one type with the same name or GUID already exists. 

