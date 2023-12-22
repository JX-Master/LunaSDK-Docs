# Luna::register_enum_type

```c++
template <typename _Ty>
typeinfo_t register_enum_type(Span< const EnumerationOptionDesc > options, bool multienum=false)
```

Registers one enumeration type to the type system. The enumeration type must have one [luenum](group___runtime_type_1gaa5c575c676819bd6348365fba48b6769.md) macro defined directly in `Luna` namespace. 



## Parameters
* *in* **options**

    A list of options that should be tracked by the type system. The user can use [luoption](group___runtime_type_1ga2c3ef7a6cd6e691e08c11d97650d53a5.md) macro to declare options conveniently. 

* *in* **multienum**

    Whether this enumeration type is a multi-value enumeration. See remarks of [EnumerationTypeDesc](struct_luna_1_1_enumeration_type_desc.md) for details. 

## Return value
Returns the registered structure type. 

