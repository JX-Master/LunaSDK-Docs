# Luna::register_enum_type

```c++
template <typename _Ty>
typeinfo_t register_enum_type(Span< const EnumerationOptionDesc > options, bool multienum=false)
```

Registers one enumeration type to the type system. The enumeration type must have one luenum macro defined directly in `Luna` namespace. 

## Overview


## Parameters
### options
A list of options that should be tracked by the type system. The user can use luoption macro to declare options conveniently. 

### multienum
Whether this enumeration type is a multi-value enumeration. See remarks of [EnumerationTypeDesc](struct_luna_1_1_enumeration_type_desc.md) for details. 

## Return value
Returns the registered structure type. 

