# Luna::VariantType::string

```c++
string = 4
```

Indicates a string variant. 

A string variant contains one string represented by a [Name](class_luna_1_1_name.md) object. You can fetch the underlying string by calling [Variant::str](class_luna_1_1_variant_1ac8fe692e37d0123f87e9408e3074b827.md) or [Variant::c_str](class_luna_1_1_variant_1ad3055a47184109b17c16c9b7465a1fec.md), the former one returns one [Name](class_luna_1_1_name.md) object while the later one returns one C-style string (`const c8*`). 

