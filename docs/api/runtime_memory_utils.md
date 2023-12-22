# Memory utility library
## Types
* [Luna::Unconstructed](class_luna_1_1_unconstructed.md)

    Represents one object that supports manual construction and destruction. 


* [Luna::MemoryLayoutMember](struct_luna_1_1_memory_layout_member.md)

    Describes one member used by memory layouting algorithms. 


## Functions
* [void * memzero(void *dst, usize byte_count)](group___runtime_memory_utils_1ga21ab8d9fe0fe13c23177a91111cccd65.md)

    Clears the specified memory region to 0. 

* [_Ty * memzero(_Ty *dst)](group___runtime_memory_utils_1gae8b5a7ce4c407bbaddac2fa58d7a30ef.md)

    Clears the memory of the specified object to 0. 

* [void * memcpy_bitmap(void *dst, const void *src, usize copy_size_per_row, usize num_rows, usize dst_row_pitch, usize src_row_pitch)](group___runtime_memory_utils_1ga78167f1e50bc8e09715866d8c36140f8.md)

    Copies the data for a 2D bitmap. 

* [void * memcpy_bitmap3d(void *dst, const void *src, usize copy_size_per_row, usize num_rows, usize num_slices, usize dst_row_pitch, usize src_row_pitch, usize dst_slice_pitch, usize src_slice_pitch)](group___runtime_memory_utils_1ga2084d1865994d1530d4ed36a940cedf5.md)

    Copies the data for a 3D bitmap. 

* [void * pixel_offset(void *base, usize x, usize y, usize z, usize bytes_per_pixel, usize row_pitch, usize slice_pitch)](group___runtime_memory_utils_1ga0fc5695a322734022f1a887933f4f8d6.md)

    Returns a pointer that offsets the specified pixels in the bitmap. 

* [const void * pixel_offset(const void *base, usize x, usize y, usize z, usize bytes_per_pixel, usize row_pitch, usize slice_pitch)](group___runtime_memory_utils_1gaf3c69cb13eff1f1f10e6a0a4a4b307b8.md)

    Returns a pointer that offsets the specified pixels in the bitmap. 

* [constexpr unsigned long long operator""_kb(unsigned long long v)](group___runtime_memory_utils_1ga20408cbb7d15561150338b30cdad1aa7.md)

    A integer literal suffix that multiples one number with 1024. Use it like `3_kb`. 

* [constexpr unsigned long long operator""_mb(unsigned long long v)](group___runtime_memory_utils_1ga99a857fef948b5282d2b7a8615aa4f6f.md)

    A integer literal suffix that multiples one number with 1024 * 1024. Use it like `3_mb`. 

* [constexpr unsigned long long operator""_gb(unsigned long long v)](group___runtime_memory_utils_1ga179f7247b699a3cd0a12ded569cb22db.md)

    A integer literal suffix that multiples one number with 1024 * 1024 * 1024. Use it like `3_gb`. 

* [constexpr unsigned long long operator""_tb(unsigned long long v)](group___runtime_memory_utils_1ga883bca1e3e4c74e7a5518d4efd77f450.md)

    A integer literal suffix that multiples one number with 1024 * 1024 * 1024 * 1024. Use it like `3_tb`. 

* [bool bit_test(const void *base_addr, usize bit_offset)](group___runtime_memory_utils_1gaacaed16341185899ffe0d769237104f2.md)

    Tests if specified bit is 1. 

* [void bit_set(void *addr, usize bit_offset)](group___runtime_memory_utils_1ga92aea26ede77acd254d90f668e0250ef.md)

    Sets the specified bit to 1. 

* [void bit_reset(void *addr, usize bit_offset)](group___runtime_memory_utils_1gac1d215202704b075901d5fdb7a31f27d.md)

    Sets the specified bit to 0. 

* [void bit_set(void *addr, usize bit_offset, bool value)](group___runtime_memory_utils_1gaad21944619c742f48231d090194ce3b0.md)

    Sets the specified bit to 1 if `value` is `true`, or to 0 if `value` is `false`. 

* [constexpr _Ty1 align_upper(_Ty1 origin, _Ty2 alignment)](group___runtime_memory_utils_1gaf3a51fa286a5f834344de34d0b3faa29.md)

    Returns the address/size that aligns the origin address/size to the nearest matched aligned address/size that is greater than or equal to the the origin address/size. 

* [_Ty * addressof(_Ty &value)](group___runtime_memory_utils_1gaead7e7ca97779e77866f1d76b3e1ae8e.md)

    Gets the real address for object or function `value`, even if the `operator&` of the object has been overloaded. 

* [void default_construct(_Iter dst)](group___runtime_memory_utils_1ga8df6e6633f16f6f0e07dd0e8f065deb8.md)

    Calls the default constructor for the object. 

* [void value_construct(_Iter dst)](group___runtime_memory_utils_1gab54fd1f9efa8c49a3404616ee151d35a.md)

    Calls the value constructor for the object. 

* [void copy_construct(_Iter1 dst, _Iter2 src)](group___runtime_memory_utils_1ga4fcba1cb4b0fc69fcefdbe51ae92d5d4.md)

    Calls the copy constructor for the object. 

* [void move_construct(_Iter1 dst, _Iter2 src)](group___runtime_memory_utils_1ga53e63f6749997e37e7f8da11e68a4ce1.md)

    Calls the move constructor for the object. 

* [void direct_construct(_Iter dst, _Args &&... args)](group___runtime_memory_utils_1ga7f83a4d50176950eae166cc199de2929.md)

    Calls the direct constructor for the object. 

* [void destruct(_Iter dst)](group___runtime_memory_utils_1ga01d4057e7a6026e025cbc30d10d60f89.md)

    Calls the destructor of the object. 

* [void copy_assign(_Iter1 dst, _Iter2 src)](group___runtime_memory_utils_1ga7cc40d476affed8c5cd975d060e001e9.md)

    Calls the copy assignment operator of the object. 

* [void move_assign(_Iter1 dst, _Iter2 src)](group___runtime_memory_utils_1gaa8b289f3d7d9f065c321101ec2ce0ab6.md)

    Calls the move assignment operator of the object. 

* [auto default_construct_range(_Iter first, _Iter last) -> enable_if_t< Impl::default_construct_range_is_value_type_class< _Iter >::value, void >](group___runtime_memory_utils_1gadb9e5fb1e9a0d0ba6b3a53c478bc1d25.md)

    Default-constructs a range of objects. 

* [auto value_construct_range(_Iter *first, _Iter *last) -> enable_if_t< Impl::value_construct_range_is_value_type_trivial< _Iter >::value, void >](group___runtime_memory_utils_1ga7f7cc883d2158a3bcce60a804a4f6266.md)

    Value-constructs a range of objects. 

* [auto copy_construct_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t<!Impl::copy_construct_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >](group___runtime_memory_utils_1gaae4bda0b6285b9b4c757534fdf99ea94.md)

    Copy-constructs a range of objects. 

* [auto copy_construct_range_n(_Iter1 first, usize count, _Iter2 d_first) -> enable_if_t<!Impl::copy_construct_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >](group___runtime_memory_utils_1ga34b6950d39deaf037807db6f0804efb8.md)

    Copy-constructs a range of objects. The range is provided by first object and object count. 

* [auto move_construct_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t< Impl::move_construct_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >](group___runtime_memory_utils_1ga94d2203ccaa43a601091490af58fc272.md)

    Move-constructs a range of objects. 

* [auto destruct_range(_Iter first, _Iter last) -> enable_if_t< Impl::destruct_range_is_value_type_trivial< _Iter >::value, void >](group___runtime_memory_utils_1ga64eceb1029aa97297c1eac27df9da0ef.md)

    Destructs every object in the range. 

* [auto copy_assign_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t<!Impl::copy_assign_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >](group___runtime_memory_utils_1gafa31716cbdd53a44b1ab5bf5289ebd34.md)

    Performs copy assignment operation on every object in the destination range using the corresponding object in the source range. 

* [auto move_assign_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t<!Impl::move_assign_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >](group___runtime_memory_utils_1ga2922440bc8a0efbe2c479e0b9d710a91.md)

    Performs move assignment operation on every object in the destination range using the corresponding object in the source range. 

* [auto move_assign_range_backward(_Iter1 first, _Iter1 last, _Iter2 d_last) -> enable_if_t<!Impl::move_assign_range_backward_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >](group___runtime_memory_utils_1ga545f4f89af4c04db356b321ce0711771.md)

    Same as [move_assign_range](group___runtime_memory_utils_1ga2922440bc8a0efbe2c479e0b9d710a91.md), but performs the move assign from back to front. 

* [_Iter1 fill_construct_range(_Iter1 first, _Iter1 last, const _Ty &value)](group___runtime_memory_utils_1ga8dd1b61c0dd3d9efdd8c23e0cb42afe4.md)

    Performs copy construct on each of the object in the range by taking a copy of the provided object. 

* [_Iter1 fill_assign_range(_Iter1 first, _Iter1 last, const _Ty &value)](group___runtime_memory_utils_1ga3e9313d372b263d059cb71cb3d65a8a9.md)

    Performs copy assignment on each of the object in the range by taking a copy of the provided object. 

* [auto copy_relocate_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t< Impl::copy_relocate_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >](group___runtime_memory_utils_1gab176a0253de8e05b3ff0c9d5c3bb0f04.md)

    Relocates objects in the source range to a new range that is not overlap with the source range. 

* [auto copy_relocate(_Iter1 dst, _Iter2 src) -> enable_if_t< Impl::copy_relocate_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter1 >](group___runtime_memory_utils_1ga3e53bc2228e4cc4428d755c146893c4c.md)

    Relocates one object. 

* [auto move_relocate_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t< Impl::move_relocate_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >](group___runtime_memory_utils_1ga63af54bbd0fa7737dc2d6b7a6d16e7fa.md)

    Relocates objects in the source range to a new range. 

* [auto move_relocate_range_backward(_Iter1 first, _Iter1 last, _Iter2 d_last) -> enable_if_t< Impl::move_relocate_backward_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >](group___runtime_memory_utils_1ga79d1c70e7f2da5dd53b7b58570886bd4.md)

    Relocates objects in the source range to a new range. 

* [void calculate_struct_memory_layout(Span< MemoryLayoutMember > members, usize &out_size, usize &out_alignment)](group___runtime_memory_utils_1gac90c9d2773f735a70e55915afaf969e4.md)

    Calculates the size, alignment and memory layout for one structure type. 

* [void calculate_union_memory_layout(Span< MemoryLayoutMember > members, usize &out_size, usize &out_alignment)](group___runtime_memory_utils_1ga26be5f1c4c2d9fc1735e3b6260426c42.md)

    Calculates the size, alignment and memory layout for one union type. 

