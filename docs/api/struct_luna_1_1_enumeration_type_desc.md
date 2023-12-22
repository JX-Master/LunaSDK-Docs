# Luna::EnumerationTypeDesc
Describes one enumeration type. 

```c++
struct Luna::EnumerationTypeDesc
```

## Member objects
* [Guid guid](struct_luna_1_1_enumeration_type_desc_1a0c8f65c9d3118ff62b1d40950e5154f8.md)

    The GUID of the enumeration type. This should be unique for every type. 

* [Name name](struct_luna_1_1_enumeration_type_desc_1a7082db574ba2d2d69ccafb060398b7d8.md)

    The name of the enumeration type. 

* [Name alias](struct_luna_1_1_enumeration_type_desc_1aab3519e6b2915ade2b650f777b994121.md)

    The alias of the enumeration type. This can be empty. The alias is used to identify types with the same name. This can be used for generic specialization types. 

* [typeinfo_t underlying_type](struct_luna_1_1_enumeration_type_desc_1af89fc3440a240432937a3b0c7d264963.md)

    The underlying type of the enumeration, which is the type that the enumeration value is stored as. This type must be a primitive integer type. 

* [Span<const EnumerationOptionDesc> options](struct_luna_1_1_enumeration_type_desc_1a7072b26b211d14db63c0490964878d81.md)

    A list of options for this enumeration. 

* [bool multienum](struct_luna_1_1_enumeration_type_desc_1a0d0e41840163c5554391d4f5802372d0.md)

    Whether this enumeration is a multi-value enumeration. A multi-value enumeration uses one unique bit of the value for every possible option, while a single-value enumeration uses one unique value for every possible option. For example, for one enumeration with `u16` underlying type, 16 possible options may present if the enumeration is a multi-value enumeration, and 65536 possible options may present if the enumeration is a noral enumeration. 

