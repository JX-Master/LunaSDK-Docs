# Luna::Variant::operator==

```c++
bool operator==(const Variant &rhs) const
```

Compares two variant for equality. 



## Parameters
* *in* **rhs**

    The variant to compare. 

## Return value
Returns `true` if two variants are equal. Returns `false` otherwise. 

## Remark
The comparison is proceeded as follows:1. If `this->type() != ths.type()`, returns `false`.

1. Otherwise, checks the type of the variant:1. If `type()` is `VariantType::null`, returns `true`.

1. If `type()` is `VariantType::object`, returns `true` if two variants have the same key-value pairs. Every element of `rhs` will be compared with the element with the same key in `*this` recursively.

1. If `type()` is `VariantType::array`, returns `true` if two variants have the same array data and size. Every element will be compared with the element with the same index in `*this` recursively.

1. If `type()` is `VariantType::number`, returns `true` if two variants have the same number type and value.

1. If `type()` is `VariantType::string`, returns `true` if two variants have the same string data. The string data is compared by comparing the underlying [Name](class_luna_1_1_name.md) objects that contain the string.

1. If `type()` is `VariantType::boolean`, returns `true` if two variants have the same Boolean value.

1. If `type()` is `VariantType::blob`, returns `true` if two variants have the same blob data. The blob data is compared using memcmp. 

