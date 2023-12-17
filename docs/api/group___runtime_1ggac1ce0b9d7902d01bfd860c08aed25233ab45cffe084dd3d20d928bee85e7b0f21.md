# Luna::VariantType::string

```c++
string = 4
```

Indicates a string variant. A string variant contains one string represented by a [Name](class_luna_1_1_name.md) object. You can fetch the underlying string by calling Variant::str or Variant::c_str, the former one returns one [Name](class_luna_1_1_name.md) object while the later one returns one C-style string (`const c8*`). 

