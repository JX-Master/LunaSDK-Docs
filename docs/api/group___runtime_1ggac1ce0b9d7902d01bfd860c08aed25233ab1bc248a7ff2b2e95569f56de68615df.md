# Luna::VariantType::number

```c++
number = 3
```

Indicates a number variant. A number variant stores a number of integer or floating-point type. The number type of one number variant is represented by [VariantNumberType](group___runtime_1ga736977eb95737aa8503b91d026bac3fa.md) and can be fetched by calling Variant::number_type method. The number value of the variant can be fetched by calling Variant::unum, Variant::inum and Variant::fnum methods, each of them returns the underlying number in specified format with implicit number type conversion when needed. 

