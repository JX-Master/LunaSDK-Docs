# Luna::VariantNumberType

```c++
enum VariantNumberType : u8
{
    not_number= 0
    number_i64= 1
    number_u64= 2
    number_f64= 3
}
```

Defines all possible number types of one number variant. 



## Remark
To fetch the number type of one number variant, call [Variant::number_type](class_luna_1_1_variant_1a9724594c45d6648adc44a15aae2beb75.md). 

## Options
* [not_number](group___runtime_1gga736977eb95737aa8503b91d026bac3faae019afae0df74b130c16579f822e33ae.md)

    This variant is not a number variant. 

* [number_i64](group___runtime_1gga736977eb95737aa8503b91d026bac3faaa4551cc8dc0bc8fd9be9bc9da7c7ab5c.md)

    The number is stored in signed 64-bit integer format. 

* [number_u64](group___runtime_1gga736977eb95737aa8503b91d026bac3faae67f812e1892ff4108ec859bad6f3f79.md)

    The number is stored in unsigned 64-bit integer format. 

* [number_f64](group___runtime_1gga736977eb95737aa8503b91d026bac3faa5df3578aaccdafbbd5964dd3a0c37bae.md)

    The number is stored in 64-bit floating-point format. 

