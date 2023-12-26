# Luna::Variant
Represents a dynamic typed object that stores data in a schema-less (self-described) manner. 

```c++
class Luna::Variant
```

## Member functions
* [Variant(VariantType type=VariantType::null)](class_luna_1_1_variant_1abdfff5ef9efa2e0a8d871ebc7b678476.md)

    Initializes one empty variant with the specified variant type. 

* [Variant(const Variant &rhs)](class_luna_1_1_variant_1a242c1ed4ab17f2e07a5826128ca500b1.md)

    Initializes one variant by coping data from another variant. 

* [Variant(Variant &&rhs)](class_luna_1_1_variant_1a6a63a831da5b8947f5f158996dc4853d.md)

    Initializes one variant by moving data from another variant. 

* [Variant(i64 v)](class_luna_1_1_variant_1a054da0b0038f63f353ee3ad30a96ba5e.md)

    Initializes one variant of [VariantType::number](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab1bc248a7ff2b2e95569f56de68615df.md) and [VariantNumberType::number_i64](group___runtime_1gga736977eb95737aa8503b91d026bac3faaa4551cc8dc0bc8fd9be9bc9da7c7ab5c.md) and sets its data to the specified value. 

* [Variant(u64 v)](class_luna_1_1_variant_1a075395840e1c6cdba754999bd1c29910.md)

    Initializes one variant of [VariantType::number](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab1bc248a7ff2b2e95569f56de68615df.md) and [VariantNumberType::number_u64](group___runtime_1gga736977eb95737aa8503b91d026bac3faae67f812e1892ff4108ec859bad6f3f79.md) and sets its data to the specified value. 

* [Variant(f64 v)](class_luna_1_1_variant_1a889d4bfb443ce645fd415237a65a882f.md)

    Initializes one variant of [VariantType::number](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab1bc248a7ff2b2e95569f56de68615df.md) and [VariantNumberType::number_f64](group___runtime_1gga736977eb95737aa8503b91d026bac3faa5df3578aaccdafbbd5964dd3a0c37bae.md) and sets its data to the specified value. 

* [Variant(const Name &v)](class_luna_1_1_variant_1a519eaba9bd9ab44a586ebabe46853363.md)

    Initializes one variant of [VariantType::string](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab45cffe084dd3d20d928bee85e7b0f21.md) and sets its data to the specified value. 

* [Variant(Name &&v)](class_luna_1_1_variant_1a845afddffb020205321d1cc5372a7f03.md)

    Initializes one variant of [VariantType::string](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab45cffe084dd3d20d928bee85e7b0f21.md) and sets its data to the specified value. 

* [Variant(const c8 *v)](class_luna_1_1_variant_1a9e6bb49e2e978706b3ec3044d25c85ed.md)

    Initializes one variant of [VariantType::string](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab45cffe084dd3d20d928bee85e7b0f21.md) and sets its data to the specified value. 

* [Variant(bool v)](class_luna_1_1_variant_1adfb9603a543927091461dd72d9f81a20.md)

    Initializes one variant of [VariantType::boolean](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233a84e2c64f38f78ba3ea5c905ab5a2da27.md) and sets its data to the specified value. 

* [Variant(const Blob &blob_data)](class_luna_1_1_variant_1ac7f6bb255e477b41e3ca52d448ee507a.md)

    Initializes one variant of [VariantType::blob](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233aee26908bf9629eeb4b37dac350f4754a.md) and sets its data to the specified value. 

* [Variant(Blob &&blob_data)](class_luna_1_1_variant_1a057f9f7c5332517d96b41e496028f26f.md)

    Initializes one variant of [VariantType::blob](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233aee26908bf9629eeb4b37dac350f4754a.md) and sets its data to the specified value. 

* [Variant & operator=(const Variant &rhs)](class_luna_1_1_variant_1a93fa1c5202335b16e3a0b2cbf79ec811.md)

    Assigns one variant by coping data from another variant. 

* [Variant & operator=(Variant &&rhs)](class_luna_1_1_variant_1aae6e6b3de228f7b2a03358ec8d667337.md)

    Assigns one variant by moving data from another variant. 

* [Variant & operator=(u64 v)](class_luna_1_1_variant_1a4960bcb9d74998e5df5c4898e7c20ab6.md)

    Assigns one variant with one number. The variant type will be [VariantType::number](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab1bc248a7ff2b2e95569f56de68615df.md) and [VariantNumberType::number_u64](group___runtime_1gga736977eb95737aa8503b91d026bac3faae67f812e1892ff4108ec859bad6f3f79.md) after this assignment. 

* [Variant & operator=(i64 v)](class_luna_1_1_variant_1a379ef29f28c13ee692578aeedfdbd524.md)

    Assigns one variant with one number. The variant type will be [VariantType::number](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab1bc248a7ff2b2e95569f56de68615df.md) and [VariantNumberType::number_i64](group___runtime_1gga736977eb95737aa8503b91d026bac3faaa4551cc8dc0bc8fd9be9bc9da7c7ab5c.md) after this assignment. 

* [Variant & operator=(f64 v)](class_luna_1_1_variant_1a78e5b9e1fac204bc0565bee7bc42044f.md)

    Assigns one variant with one number. The variant type will be [VariantType::number](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab1bc248a7ff2b2e95569f56de68615df.md) and [VariantNumberType::number_f64](group___runtime_1gga736977eb95737aa8503b91d026bac3faa5df3578aaccdafbbd5964dd3a0c37bae.md) after this assignment. 

* [Variant & operator=(const Name &v)](class_luna_1_1_variant_1a0139b4bfbcc6a5ddb6dab722cbfd2b48.md)

    Assigns one variant with one string. The variant type will be [VariantType::string](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab45cffe084dd3d20d928bee85e7b0f21.md) after this assignment. 

* [Variant & operator=(Name &&v)](class_luna_1_1_variant_1aba808de5b88e0a735caa880845262111.md)

    Assigns one variant with one string. The variant type will be [VariantType::string](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab45cffe084dd3d20d928bee85e7b0f21.md) after this assignment. 

* [Variant & operator=(const c8 *v)](class_luna_1_1_variant_1aa0abd054c8679e18458fbd570cc255c8.md)

    Assigns one variant with one string. The variant type will be [VariantType::string](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233ab45cffe084dd3d20d928bee85e7b0f21.md) after this assignment. 

* [Variant & operator=(bool v)](class_luna_1_1_variant_1a2bc2ce9f2bc77a2302c6d44b37f4d063.md)

    Assigns one variant with one Boolean value. The variant type will be [VariantType::boolean](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233a84e2c64f38f78ba3ea5c905ab5a2da27.md) after this assignment. 

* [Variant & operator=(const Blob &blob_data)](class_luna_1_1_variant_1a0e9f94b224ab4fdf7d648d10b9613b60.md)

    Assigns one variant with one blob. The variant type will be [VariantType::blob](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233aee26908bf9629eeb4b37dac350f4754a.md) after this assignment. 

* [Variant & operator=(Blob &&blob_data)](class_luna_1_1_variant_1a5b19259f5a8ef99d76e42f49d235d754.md)

    Assigns one variant with one blob. The variant type will be [VariantType::blob](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233aee26908bf9629eeb4b37dac350f4754a.md) after this assignment. 

* [bool operator==(const Variant &rhs) const](class_luna_1_1_variant_1ae6df49b479a23e4c8b2898ebb6a0edb1.md)

    Compares two variant for equality. 

* [bool operator!=(const Variant &rhs) const](class_luna_1_1_variant_1a5f0ec7ae66948c76086142378b5cdefe.md)

    Compares two variant for non-equality. 

* [VariantType type() const](class_luna_1_1_variant_1a9d24401239f10fa7d53b0e0a53eb90b8.md)

    Gets the type of the variant. 

* [VariantNumberType number_type() const](class_luna_1_1_variant_1a9724594c45d6648adc44a15aae2beb75.md)

    Gets the number type of the variant. 

* [bool valid() const](class_luna_1_1_variant_1a315419f26d3c59fa143b49b90a019049.md)

    Checks whether the variant is valid. 

* [bool empty() const](class_luna_1_1_variant_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether the variant contains no child variant. 

* [const Variant & at(usize i) const](class_luna_1_1_variant_1a8fa6cc1d87e0d2329f21e452f6e14179.md)

    Gets the child variant when this is an array variant. 

* [Variant & at(usize i)](class_luna_1_1_variant_1a284e54c4ca0bc2bddb277c7e56183704.md)

    Gets the child variant when this is an array variant. 

* [const Variant & find(const Name &k) const](class_luna_1_1_variant_1a909a9aaa5b3827381c4de0fd89d4ba16.md)

    Gets the child variant when this is an object variant. 

* [Variant & find_or_insert(const Name &k)](class_luna_1_1_variant_1a8a9ac8c2e242926ff3f074e23adb3ff8.md)

    Gets the child variant with the specified key, or inserts one new child variant with that key if not exists. 

* [const Variant & operator[](usize i) const](class_luna_1_1_variant_1a4dd5a71ff6a0b6e154fdc95adb1afb40.md)

    Shortcut for [at](class_luna_1_1_variant_1a8fa6cc1d87e0d2329f21e452f6e14179.md). 

* [Variant & operator[](usize i)](class_luna_1_1_variant_1a4c8d2b5b5ef0bd52261bd00848077460.md)

    Shortcut for [at](class_luna_1_1_variant_1a8fa6cc1d87e0d2329f21e452f6e14179.md). 

* [const Variant & operator[](const Name &k) const](class_luna_1_1_variant_1afbdd0e0a7513b0c3700e36e7fb77c7ae.md)

    Shortcut for [find](class_luna_1_1_variant_1a909a9aaa5b3827381c4de0fd89d4ba16.md). 

* [Variant & operator[](const Name &k)](class_luna_1_1_variant_1a6e57135238f26b42fb97f97783edbc56.md)

    Shortcut for [find_or_insert](class_luna_1_1_variant_1a8a9ac8c2e242926ff3f074e23adb3ff8.md). 

* [usize size() const](class_luna_1_1_variant_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the number of the child variants of this variant. 

* [bool contains(const Name &k) const](class_luna_1_1_variant_1abfece6668a5da4fcf34c70db968a14b9.md)

    Checks whether one child variant with the specified key exists. 

* [Variant::value_enumerator values()](class_luna_1_1_variant_1a9ec0b9f83cf0ff76e450478b7697f08f.md)

    Gets one enumerator that can be used to enumerate all child variants of one array variant. 

* [Variant::const_value_enumerator values() const](class_luna_1_1_variant_1a08fac7eedea7f4b4f86eba5ff366cd24.md)

    Gets one enumerator that can be used to enumerate all child variants of one array variant. 

* [Variant::key_value_enumerator key_values()](class_luna_1_1_variant_1a0dda76c8c641eb11aaae3e87e78569a5.md)

    Gets one enumerator to enumerate all child key-variant pairs of one object variant. 

* [Variant::const_key_value_enumerator key_values() const](class_luna_1_1_variant_1ad11c7ab4067983bc2fe7f490c3909647.md)

    Gets one enumerator to enumerate all child key-variant pairs of one object variant. 

* [void insert(usize i, const Variant &val)](class_luna_1_1_variant_1a733311c3870e990aa2e7e561ff113f1c.md)

    Copy-inserts one variant to the specified index. 

* [void insert(usize i, Variant &&val)](class_luna_1_1_variant_1afbb0dc7bfaa890b590e7fc485142d25f.md)

    Move-inserts one variant to the specified index. 

* [void push_back(const Variant &val)](class_luna_1_1_variant_1a3639acb126436f8f1888ad043e498973.md)

    Copy-inserts one variant to the end of the variant array. 

* [void push_back(Variant &&val)](class_luna_1_1_variant_1affa13f4e83766862c7d3895ee6780813.md)

    Move-inserts one variant to the end of the variant array. 

* [void erase(usize i)](class_luna_1_1_variant_1a07213602e6a893ddee649a01031dce46.md)

    Removes one child variant from the current variant. 

* [void erase(usize begin, usize end)](class_luna_1_1_variant_1ab407f9532e933e933728f80c5625dfc1.md)

    Erases one range [begin, end) of child variants from the current variant. 

* [void pop_back()](class_luna_1_1_variant_1a058bda4957df6a97b1ea6c9fd783f672.md)

    Erases the last child variant from the child variants array of the current variant. 

* [bool insert(const Name &k, const Variant &val)](class_luna_1_1_variant_1a0368fa4d866e320be06a5a6c89e2b5f6.md)

    Copy-inserts the variant with the specified key as the child variant of the current variant. 

* [bool insert(const Name &k, Variant &&val)](class_luna_1_1_variant_1ac550a8c8d602c13a346e6740b5ba65b5.md)

    Move-inserts the variant with the specified key as the child variant of the current variant. 

* [bool erase(const Name &k)](class_luna_1_1_variant_1af09c24b91391a20bad750622b2472795.md)

    Removes the child variant with the specified key from the current variant. 

* [Name str(const Name &default_value=Name()) const](class_luna_1_1_variant_1ac8fe692e37d0123f87e9408e3074b827.md)

    Gets the string of one string variant. 

* [const c8 * c_str(const c8 *default_value="") const](class_luna_1_1_variant_1ad3055a47184109b17c16c9b7465a1fec.md)

    Gets the C string of one string variant. 

* [i64 inum(i64 default_value=0) const](class_luna_1_1_variant_1a466199d73f82566eb5ca63bee27eee87.md)

    Gets the data of one number variant as one signed 64-bit integer. 

* [u64 unum(u64 default_value=0) const](class_luna_1_1_variant_1ad1821756df92efe114b351fc1ec42993.md)

    Gets the data of one number variant as one unsigned 64-bit integer. 

* [f64 fnum(f64 default_value=0) const](class_luna_1_1_variant_1a860281cf7826d8e4f76264a2aeb11ab0.md)

    Gets the data of one number variant as one 64-bit floating-point number. 

* [bool boolean(bool default_value=false) const](class_luna_1_1_variant_1a64ba360acf25cc61985213c4c0934520.md)

    Gets the data of one Boolean variant. 

* [byte_t * blob_data()](class_luna_1_1_variant_1ae3fc3887c6b13778183226f9e2207087.md)

    Gets the data pointer of one BLOB variant. 

* [const byte_t * blob_data() const](class_luna_1_1_variant_1a5645dc816c98ce8a7436b7a42cb749a5.md)

    Gets the data pointer of one BLOB variant. 

* [usize blob_size() const](class_luna_1_1_variant_1a3e5b168557975c0111113042905dc6fd.md)

    Gets the data size, in bytes, of one BLOB variant. 

* [usize blob_alignment() const](class_luna_1_1_variant_1a97d689d00955729db2ed0dfa2bb47128.md)

    Gets the data alignment, in bytes, of one BLOB variant. 

* [Blob blob_detach()](class_luna_1_1_variant_1af0abd7cebd9b92bb336b3ca799f6a83e.md)

    Detaches and gets the data of one BLOB variant as a [Blob](class_luna_1_1_blob.md) object. 

