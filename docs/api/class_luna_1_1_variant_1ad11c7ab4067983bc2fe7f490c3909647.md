# Luna::Variant::key_values

```c++
Variant::const_key_value_enumerator key_values() const
```

Gets one enumerator to enumerate all child key-variant pairs of one object variant. 



## Return value
Returns one enumerator to enumerate all child key-variant pairs. Returns one enumerator with an empty range if [type](class_luna_1_1_variant_1a9d24401239f10fa7d53b0e0a53eb90b8.md) of the variant is not [VariantType::object](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233aa8cfde6331bd59eb2ac96f8911c4b666.md). 

## Remark
The returned enumerator will have `begin` and `end` methods that can be used like all other containers in Luna SDK. You can also use the enumerator in a range-based for loop like so: 
```
for (auto& i : variant.[key_values](class_luna_1_1_variant_1a0dda76c8c641eb11aaae3e87e78569a5.md)())
{
    [i](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a865c0c0b4ab0e063e5caa3387c1a8741.md).first; // key.
       [i](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a865c0c0b4ab0e063e5caa3387c1a8741.md).second; // value.
}[s](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a03c7c0ace395d80182db07ae2c30f034.md)
```


