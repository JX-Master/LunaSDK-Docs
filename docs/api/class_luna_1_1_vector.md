# Luna::Vector
A container that stores a continuous array of elements. Elements can be added to or removed from the container dynamically. 

```c++
template <typename _Ty, typename _Alloc>
class Luna::Vector
```



## Parameters
* **_Ty**

    The element type of the container. 

* **_Alloc**

    The memory allocator used by the container. If not specified, [Allocator](class_luna_1_1_allocator.md) will be used. 

## Member functions
* [Vector()](class_luna_1_1_vector_1a4df026156780bc0ca651c342b7d6daa4.md)

    Constructs an empty vector. 

* [Vector(const allocator_type &alloc)](class_luna_1_1_vector_1a1edb33677a1ff398bb1cdf967eb49f43.md)

    Constructs an empty vector with an custom allocator. 

* [Vector(usize count, const value_type &value, const allocator_type &alloc=allocator_type())](class_luna_1_1_vector_1aece5483d043a7ee18785b66c2a0bd393.md)

    Constructs one vector with `count` elements, with their values initialized by `value`. 

* [Vector(usize count, const allocator_type &alloc=allocator_type())](class_luna_1_1_vector_1a8d1c8fb80795ba2377e1f10359eb9c12.md)

    Constructs one vector with `count` elements, which their values being default-initialized. 

* [Vector(enable_if_t<!is_integral_v< _InputIt >, _InputIt > first, _InputIt last, const allocator_type &alloc=allocator_type())](class_luna_1_1_vector_1a4b30c1bff8cc47be5ab78651638ea3f4.md)

    Constructs one vector with elements copied from the specified range. 

* [Vector(const Vector &rhs)](class_luna_1_1_vector_1a3a8333eacded76335c362842f60e2c68.md)

    Constructs a vector by copying elements from another vector. 

* [Vector(const Vector &rhs, const allocator_type &alloc)](class_luna_1_1_vector_1a80d91bac4539822049bf996b6830449c.md)

    Constructs a vector with an custom allocator and with elements copied from another vector. 

* [Vector(Vector &&rhs)](class_luna_1_1_vector_1a3925af7d7ef4f89d96474e23b2b3c169.md)

    Constructs a vector by moving elements from another vector. 

* [Vector(Vector &&rhs, const allocator_type &alloc)](class_luna_1_1_vector_1a6c6e46dbf5d0d3459655f1affca87b97.md)

    Constructs a vector with an custom allocator and with elements moved from another vector. 

* [Vector(InitializerList< value_type > init, const allocator_type &alloc=allocator_type())](class_luna_1_1_vector_1a74cc918f6f6aa3a302d9b9fcaed455c7.md)

    Constructs one vector by coping all elements from an initializer list. 

* [Vector< _Ty, _Alloc > & operator=(const Vector &rhs)](class_luna_1_1_vector_1a09d298b36599b33578e4aba16293f7c6.md)

    Replaces elements of the vector by coping elements from another vector. 

* [Vector< _Ty, _Alloc > & operator=(Vector &&rhs)](class_luna_1_1_vector_1a559f1b48413087bfc71e5bb5a2ad1c28.md)

    Replaces elements of the vector by moving elements from another vector. 

* [Vector< _Ty, _Alloc > & operator=(InitializerList< value_type > ilist)](class_luna_1_1_vector_1a277727d1e1803a420b39b47e6b7240b9.md)

    Replaces elements of the vector from one initializer list. 

* [Vector< _Ty, _Alloc >::iterator begin()](class_luna_1_1_vector_1a02a9804e8ea9ee5c51527c2b07fe8aeb.md)

    Gets one iterator to the first element of the vector. 

* [Vector< _Ty, _Alloc >::iterator end()](class_luna_1_1_vector_1a858bae9b8e39c8395873a958a01aa0d0.md)

    Gets one iterator to the one past last element of the vector. 

* [Vector< _Ty, _Alloc >::const_iterator begin() const](class_luna_1_1_vector_1addfe5102c0f3450e910bc6a6f4d221b2.md)

    Gets one constant iterator to the first element of the vector. 

* [Vector< _Ty, _Alloc >::const_iterator end() const](class_luna_1_1_vector_1a75d29b65d11867c5ed1eca0a28c0f9c6.md)

    Gets one constant iterator to the one past last element of the vector. 

* [Vector< _Ty, _Alloc >::const_iterator cbegin() const](class_luna_1_1_vector_1a6dde9da4184a08238b64631900e41582.md)

    Gets one constant iterator to the first element of the vector. 

* [Vector< _Ty, _Alloc >::const_iterator cend() const](class_luna_1_1_vector_1a6aae92acd25f13f5b45fffcb2c408611.md)

    Gets one constant iterator to the one past last element of the vector. 

* [Vector< _Ty, _Alloc >::reverse_iterator rbegin()](class_luna_1_1_vector_1aba9ce1a0d36b4cc5f1b54f6977603fb3.md)

    Gets one reverse iterator to the last element of the vector. 

* [Vector< _Ty, _Alloc >::reverse_iterator rend()](class_luna_1_1_vector_1ae3c62fd959c35389959c590e3a17fa2f.md)

    Gets one reverse iterator to the one-before-first element of the vector. 

* [Vector< _Ty, _Alloc >::const_reverse_iterator rbegin() const](class_luna_1_1_vector_1aef1d5823f755f9f9f842c727b33e5e96.md)

    Gets one constant reverse iterator to the last element of the vector. 

* [Vector< _Ty, _Alloc >::const_reverse_iterator rend() const](class_luna_1_1_vector_1a1e1ef2026cbe5bc8c57b4c3a4f04606d.md)

    Gets one constant reverse iterator to the one-before-first element of the vector. 

* [Vector< _Ty, _Alloc >::const_reverse_iterator crbegin() const](class_luna_1_1_vector_1a624f516269312247f3786c96653f958a.md)

    Gets one constant reverse iterator to the last element of the vector. 

* [Vector< _Ty, _Alloc >::const_reverse_iterator crend() const](class_luna_1_1_vector_1af2d071dd47c6731a48a3e2153c1ec399.md)

    Gets one constant reverse iterator to the one-before-first element of the vector. 

* [usize size() const](class_luna_1_1_vector_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the vector, that is, the number of elements in the vector. 

* [usize capacity() const](class_luna_1_1_vector_1ad96bf59cb22e917cbd210ba068e8acb3.md)

    Gets the capacity of the vector, that is, the maximum number of elements this vector can hold before next expansion. 

* [bool empty() const](class_luna_1_1_vector_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this vector is empty, that is, the size of this vector is `0`. 

* [void reserve(usize new_cap)](class_luna_1_1_vector_1aa1c32ac6498d3f6d21cab98d1cbf3455.md)

    Increases the capacity of the vector to a value greater than or equal to `new_cap`, so that it can hold at least `new_cap` elements without reallocating the internal buffer. 

* [void resize(usize n)](class_luna_1_1_vector_1a958e85419f9a79f27716d410e54151a5.md)

    Resizes the vector. 

* [void resize(usize n, const value_type &v)](class_luna_1_1_vector_1a9ac9a00e56a979fc38a2970a573f3868.md)

    Resizes the vector. 

* [void shrink_to_fit()](class_luna_1_1_vector_1a5f16304f80b6fb253c7b0ead3e16dd18.md)

    Reduces the capacity of the vector so that [capacity](class_luna_1_1_vector_1ad96bf59cb22e917cbd210ba068e8acb3.md) == [size](class_luna_1_1_vector_1a79348f1b7c06b34052b42656a0279429.md). 

* [Vector< _Ty, _Alloc >::reference operator[](usize n)](class_luna_1_1_vector_1a7c38718520fc07f97c3714c03e0d0c62.md)

    Gets the element at the specified index. 

* [Vector< _Ty, _Alloc >::const_reference operator[](usize n) const](class_luna_1_1_vector_1ab3e774acb8e4111bd3a7c6b2276d4e0d.md)

    Gets the element at the specified index. 

* [Vector< _Ty, _Alloc >::reference at(usize n)](class_luna_1_1_vector_1a20f5c77bf6904e3fe5275457bc6ae43a.md)

    Gets the element at the specified index. 

* [Vector< _Ty, _Alloc >::const_reference at(usize n) const](class_luna_1_1_vector_1ace1550e61dd4fa67622be6e19c65ebbb.md)

    Gets the element at the specified index. 

* [Vector< _Ty, _Alloc >::reference front()](class_luna_1_1_vector_1a5af3831bb9d9b945f4214965240b8333.md)

    Gets the element at the front of the vector. 

* [Vector< _Ty, _Alloc >::const_reference front() const](class_luna_1_1_vector_1a7d9ff8ea72340566ccbde197b6ec81c2.md)

    Gets the element at the front of the vector. 

* [Vector< _Ty, _Alloc >::reference back()](class_luna_1_1_vector_1ad878097e40e9795bd6659f4bad0ab39c.md)

    Gets the element at the back of the vector. 

* [Vector< _Ty, _Alloc >::const_reference back() const](class_luna_1_1_vector_1ade864f1a478ee06c4392c68b6277a2c1.md)

    Gets the element at the back of the vector. 

* [Vector< _Ty, _Alloc >::pointer data()](class_luna_1_1_vector_1af4377b72b6645e313e1f6b51330d33af.md)

    Gets one pointer to the data buffer of this vector. 

* [Vector< _Ty, _Alloc >::const_pointer data() const](class_luna_1_1_vector_1a43786b42323390d7c8ef2238ad6aa641.md)

    Gets one pointer to the data buffer of this vector. 

* [void clear()](class_luna_1_1_vector_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all elements from the vector, but keeps the vector storage. 

* [void push_back(const value_type &val)](class_luna_1_1_vector_1a39f502e5f35796bfbfc13e04a3fe5273.md)

    Pushes one element to the back of the vector. 

* [void push_back(value_type &&val)](class_luna_1_1_vector_1adee40331581f67476805b40ac8d80287.md)

    Pushes one element to the back of the vector. 

* [void pop_back()](class_luna_1_1_vector_1a058bda4957df6a97b1ea6c9fd783f672.md)

    Removes the element from the back of the vector. 

* [void assign(usize count, const value_type &value)](class_luna_1_1_vector_1aafc1352043c99963fa09825f1a384a10.md)

    Replaces elements of the vector by several copies of the specified value. 

* [auto assign(_InputIter first, _InputIter last) -> enable_if_t<!is_integral_v< _InputIter >, void >](class_luna_1_1_vector_1a7ab1d03fd4a0ee332bc3883252bbbb91.md)

    Replaces elements of the vector by elements specified by one range. Elements in the range will be copy-inserted into the vector. 

* [void assign(InitializerList< value_type > il)](class_luna_1_1_vector_1a41c4f74264cdfe0044cb0d1c00f28c8d.md)

    Replaces elements of the vector by elements from one initializer vector. 

* [void assign(Span< _Rty > data)](class_luna_1_1_vector_1a91f5692adeaf575f06caa3496f93841e.md)

    Replaces elements of the vector by elements specified by one span. Elements in the span will be copy-inserted into the vector. 

* [Vector< _Ty, _Alloc >::iterator insert(const_iterator pos, const value_type &value)](class_luna_1_1_vector_1a566f534394a867a68344252fe75201d4.md)

    Inserts the specified element to the vector. 

* [Vector< _Ty, _Alloc >::iterator insert(const_iterator pos, value_type &&value)](class_luna_1_1_vector_1ac2a97ddaaad0b1eeffc002b7b1df9a91.md)

    Inserts the specified element to the vector. 

* [Vector< _Ty, _Alloc >::iterator insert(const_iterator pos, usize count, const value_type &value)](class_luna_1_1_vector_1ab1326a92b868458f9540ebca746f2793.md)

    Inserts several copies of the element to the vector. 

* [auto insert(const_iterator pos, _InputIt first, _InputIt last) -> enable_if_t<!is_integral_v< _InputIt >, iterator >](class_luna_1_1_vector_1a4def82cce5edd6eaf0715925cdd6aa9a.md)

    Inserts one range of elements to the vector. 

* [Vector< _Ty, _Alloc >::iterator insert(const_iterator pos, InitializerList< value_type > ilist)](class_luna_1_1_vector_1a1c72b3dd1ee565460d5e86608fdf0ea9.md)

    Inserts one range of elements specified by the initializer list to the vector. 

* [Vector< _Ty, _Alloc >::iterator insert(const_iterator pos, Span< _Rty > data)](class_luna_1_1_vector_1a37648bc120f8ef4af2cc35a36594c8d8.md)

    Inserts elements specified by the span to the vector. Elements in the span will be copy-inserted into the vector. 

* [Vector< _Ty, _Alloc >::iterator erase(const_iterator pos)](class_luna_1_1_vector_1ad7cd3ed118f87518e4ee4025a2a0fa8f.md)

    Removes one element from the vector. 

* [Vector< _Ty, _Alloc >::iterator erase(const_iterator first, const_iterator last)](class_luna_1_1_vector_1adb1aca5cf1890c612df86f2c2cfa1317.md)

    Removes one range of elements from the vector. 

* [Vector< _Ty, _Alloc >::iterator swap_erase(const_iterator pos)](class_luna_1_1_vector_1a2d4452a0a4d7364873ee614a4b16baca.md)

    Destructs the element at specified posiiton, then relocates the last element of the vector to the specified position. 

* [void swap(Vector &rhs)](class_luna_1_1_vector_1af2331ce2a616992c051ea34b0a167a35.md)

    Swaps elements of this vector with the specified vector. 

* [Vector< _Ty, _Alloc >::iterator emplace(const_iterator pos, _Args &&... args)](class_luna_1_1_vector_1ab22441cb49b5eead35b7eaebe6b64e35.md)

    Constructs one element directly on the specified position of the vector using the provided arguments. 

* [Vector< _Ty, _Alloc >::iterator emplace_back(_Args &&... args)](class_luna_1_1_vector_1a1d88040d8fec5746bf21e282a68ec136.md)

    Constructs one element directly on the back of the vector using the provided arguments. 

* [Vector< _Ty, _Alloc >::allocator_type get_allocator() const](class_luna_1_1_vector_1a8089b36b18cac7811454fd5da9fbf1aa.md)

    Gets the allocator of the vector. 

* [Span< _Ty > span()](class_luna_1_1_vector_1af59a08bb0b5a699bf14bcfee275e5932.md)

    Creates one span that specifies the element buffer of this vector. 

* [Span< const _Ty > span() const](class_luna_1_1_vector_1a4b740c593d38cc477d2418c3717d9920.md)

    Creates one constant span that specifies the element buffer of this vector. 

* [Span< const _Ty > cspan() const](class_luna_1_1_vector_1a514d68c1e8f028317840d3d81d111182.md)

    Creates one constant span that specifies the element buffer of this vector. 

