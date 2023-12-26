# Luna::VariantType::number

```c++
number = 3
```

Indicates a number variant. 

A number variant stores a number of integer or floating-point type. The number type of one number variant is represented by [VariantNumberType](group___runtime_1ga736977eb95737aa8503b91d026bac3fa.md) and can be fetched by calling [Variant::number_type](class_luna_1_1_variant_1a9724594c45d6648adc44a15aae2beb75.md) method. The number value of the variant can be fetched by calling [Variant::unum](class_luna_1_1_variant_1ad1821756df92efe114b351fc1ec42993.md), [Variant::inum](class_luna_1_1_variant_1a466199d73f82566eb5ca63bee27eee87.md) and [Variant::fnum](class_luna_1_1_variant_1a860281cf7826d8e4f76264a2aeb11ab0.md) methods, each of them returns the underlying number in specified format with implicit number type conversion when needed. 

