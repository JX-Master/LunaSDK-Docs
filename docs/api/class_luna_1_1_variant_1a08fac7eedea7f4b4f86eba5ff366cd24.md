# Luna::Variant::values

```c++
Variant::const_value_enumerator values() const
```

Gets one enumerator that can be used to enumerate all child variants of one array variant. 



## Return value
Returns one enumerator that can be used to enumerate all child variants. Returns one enumerator with an empty range if [type](class_luna_1_1_variant_1a9d24401239f10fa7d53b0e0a53eb90b8.md) of the variant is not [VariantType::array](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233af1f713c9e000f5d3f280adbd124df4f5.md). 

## Remark
The returned enumerator will have `begin` and `end` methods that can be used like all other containers in Luna SDK. You can also use the enumerator in a range-based for loop like so: 
```
for (auto& i : variant.[values](class_luna_1_1_variant_1a9ec0b9f83cf0ff76e450478b7697f08f.md)())
{
    //...
}
```


