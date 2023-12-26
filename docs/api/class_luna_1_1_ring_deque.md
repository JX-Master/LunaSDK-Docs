# Luna::RingDeque
A container that implements a double-ended queue and uses a ring buffer as its internal storage. 

```c++
template <typename _Ty, typename _Alloc>
class Luna::RingDeque
```



## Parameters
* **_Ty**

    The element type of the container. 

* **_Alloc**

    The memory allocator used by the container. If not specified, [Allocator](class_luna_1_1_allocator.md) will be used. 

## Member functions
* [iterator begin()](class_luna_1_1_ring_deque_1ad69bd11391be1a1dba5c8202259664f8.md)

    Gets one iterator to the first element of the queue. 

* [iterator end()](class_luna_1_1_ring_deque_1acad38d52497a975bfb6f2f6acd76631f.md)

    Gets one iterator to the one past last element of the queue. 

* [const_iterator begin() const](class_luna_1_1_ring_deque_1a29305669b60ca1680752e2fc3592ba99.md)

    Gets one constant iterator to the first element of the queue. 

* [const_iterator end() const](class_luna_1_1_ring_deque_1accf9a4bd0c34d4a5f6a7dab66ea10cdc.md)

    Gets one constant iterator to the one past last element of the queue. 

* [const_iterator cbegin() const](class_luna_1_1_ring_deque_1a39112ae08f6ffc7ee58c6aa79772e094.md)

    Gets one constant iterator to the first element of the queue. 

* [const_iterator cend() const](class_luna_1_1_ring_deque_1a93791e61ab486b4022c389d634b4facc.md)

    Gets one constant iterator to the one past last element of the queue. 

* [reverse_iterator rbegin()](class_luna_1_1_ring_deque_1acea44ed500a54b2bb93e16b86e81afa8.md)

    Gets one reverse iterator to the last element of the queue. 

* [reverse_iterator rend()](class_luna_1_1_ring_deque_1a68c599ddcbfddc65170de524ac165e44.md)

    Gets one reverse iterator to the one-before-first element of the queue. 

* [const_reverse_iterator rbegin() const](class_luna_1_1_ring_deque_1af086cceac199bd735c7a97c2a8d7ed21.md)

    Gets one constant reverse iterator to the last element of the queue. 

* [const_reverse_iterator rend() const](class_luna_1_1_ring_deque_1a07da1fdc890b6949f1a20a1961c6fc44.md)

    Gets one constant reverse iterator to the one-before-first element of the queue. 

* [const_reverse_iterator crbegin() const](class_luna_1_1_ring_deque_1a81f80a31923e85af56a7b1ae0712a33b.md)

    Gets one constant reverse iterator to the last element of the queue. 

* [const_reverse_iterator crend() const](class_luna_1_1_ring_deque_1abef9dfc7607c7e1a3854788ba56a4f34.md)

    Gets one constant reverse iterator to the one-before-first element of the queue. 

* [usize size() const](class_luna_1_1_ring_deque_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the queue, that is, the number of elements in the queue. 

* [usize capacity() const](class_luna_1_1_ring_deque_1ad96bf59cb22e917cbd210ba068e8acb3.md)

    Gets the capacity of the queue, that is, the maximum number of elements this queue can hold before next expansion. 

* [bool empty() const](class_luna_1_1_ring_deque_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this queue is empty, that is, the size of this queue is `0`. 

* [RingDeque()](class_luna_1_1_ring_deque_1abc95d48513f45e35c03589e954c1bcfd.md)

    Constructs an empty queue. 

* [RingDeque(const allocator_type &alloc)](class_luna_1_1_ring_deque_1a2e95a68f196cc154c2beef40a06eccda.md)

    Constructs an empty queue with an custom allocator. 

* [RingDeque(const RingDeque &rhs)](class_luna_1_1_ring_deque_1a5945ab498b637747f439366dbf01cd0c.md)

    Constructs a queue by copying elements from another queue. 

* [RingDeque(const RingDeque &rhs, const allocator_type &alloc)](class_luna_1_1_ring_deque_1a715d083d2bc795a623618cec24733824.md)

    Constructs a queue with an custom allocator and with elements copied from another queue. 

* [RingDeque(RingDeque &&rhs)](class_luna_1_1_ring_deque_1a42fb5f861ae9e7c5d02cd7663dff5a3f.md)

    Constructs a queue by moving elements from another queue. 

* [RingDeque(RingDeque &&rhs, const allocator_type &alloc)](class_luna_1_1_ring_deque_1ad207336e681a86cdfd053a264a461c47.md)

    Constructs a queue with an custom allocator and with elements moved from another queue. 

* [RingDeque & operator=(const RingDeque &rhs)](class_luna_1_1_ring_deque_1ac7061438cfaeabd9c1b0a14342411619.md)

    Replaces elements of the queue by coping elements from another queue. 

* [RingDeque & operator=(RingDeque &&rhs)](class_luna_1_1_ring_deque_1a9aa0640b43a1e39e2dd28dcc6e24c276.md)

    Replaces elements of the queue by moving elements from another queue. 

* [void reserve(usize new_cap)](class_luna_1_1_ring_deque_1aa1c32ac6498d3f6d21cab98d1cbf3455.md)

    Increases the capacity of the queue to a value greater than or equal to `new_cap`, so that it can hold at least `new_cap` elements without reallocating the internal buffer. 

* [void resize(usize n)](class_luna_1_1_ring_deque_1a958e85419f9a79f27716d410e54151a5.md)

    Resizes the queue. 

* [void resize(usize n, const value_type &v)](class_luna_1_1_ring_deque_1a9ac9a00e56a979fc38a2970a573f3868.md)

    Resizes the queue. 

* [void shrink_to_fit()](class_luna_1_1_ring_deque_1a5f16304f80b6fb253c7b0ead3e16dd18.md)

    Reduces the capacity of the queue so that [capacity](class_luna_1_1_ring_deque_1ad96bf59cb22e917cbd210ba068e8acb3.md) == [size](class_luna_1_1_ring_deque_1a79348f1b7c06b34052b42656a0279429.md). 

* [reference operator[](usize n)](class_luna_1_1_ring_deque_1af3b723d2dfaf71d3da66ecb50acf560a.md)

    Gets the element at the specified index. 

* [const_reference operator[](usize n) const](class_luna_1_1_ring_deque_1a2c885a2ebc6a7668545533f97d0711a8.md)

    Gets the element at the specified index. 

* [reference at(usize n)](class_luna_1_1_ring_deque_1a6d0e2e0d719d566c64944e472a502823.md)

    Gets the element at the specified index. 

* [const_reference at(usize n) const](class_luna_1_1_ring_deque_1ae8807da58af6a91beb3d4466af5d3c82.md)

    Gets the element at the specified index. 

* [reference front()](class_luna_1_1_ring_deque_1a6a48363b4355f6f5b441637774f79a59.md)

    Gets the element at the front of the queue. 

* [const_reference front() const](class_luna_1_1_ring_deque_1a0ae6b4f9719202f7ddb334c16fb03d80.md)

    Gets the element at the front of the queue. 

* [reference back()](class_luna_1_1_ring_deque_1af71e6c1eccbc12e9339c00a86a981a43.md)

    Gets the element at the back of the queue. 

* [const_reference back() const](class_luna_1_1_ring_deque_1a61772c77ad2abfbb296912e7281e154c.md)

    Gets the element at the back of the queue. 

* [void clear()](class_luna_1_1_ring_deque_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all elements from the queue, but keeps the queue storage. 

* [void push_back(const value_type &val)](class_luna_1_1_ring_deque_1a39f502e5f35796bfbfc13e04a3fe5273.md)

    Pushes one element to the back of the queue. 

* [void push_back(value_type &&val)](class_luna_1_1_ring_deque_1adee40331581f67476805b40ac8d80287.md)

    Pushes one element to the back of the queue. 

* [void pop_back()](class_luna_1_1_ring_deque_1a058bda4957df6a97b1ea6c9fd783f672.md)

    Removes the element from the back of the queue. 

* [void push_front(const value_type &val)](class_luna_1_1_ring_deque_1a57f9a229b17905478897524d2918982b.md)

    Pushes one element at the front of the queue. 

* [void push_front(value_type &&val)](class_luna_1_1_ring_deque_1aa1c6105ed239f4e0cd04fecf98e0d1a3.md)

    Pushes one element at the front of the queue. 

* [void pop_front()](class_luna_1_1_ring_deque_1a56f4ffbc6fd414b3c02a6c368e99594f.md)

    Removes the element at the front of the queue. 

* [void assign(usize count, const value_type &value)](class_luna_1_1_ring_deque_1aafc1352043c99963fa09825f1a384a10.md)

    Replaces elements of the queue by several copies of the specified value. 

* [auto assign(_InputIter first, _InputIter last) -> enable_if_t<!is_integral_v< _InputIter >, void >](class_luna_1_1_ring_deque_1a7ab1d03fd4a0ee332bc3883252bbbb91.md)

    Replaces elements of the queue by elements specified by one range. Elements in the range will be copy-inserted into the queue. 

* [void assign(InitializerList< value_type > il)](class_luna_1_1_ring_deque_1a41c4f74264cdfe0044cb0d1c00f28c8d.md)

    Replaces elements of the queue by elements from one initializer queue. 

* [iterator insert(const_iterator pos, const value_type &value)](class_luna_1_1_ring_deque_1aca6516cf43b8d52176a8d5b8fb53327c.md)

    Inserts the specified element to the queue. 

* [iterator insert(const_iterator pos, value_type &&value)](class_luna_1_1_ring_deque_1a3cd54460938e9ca79d11d8afff7034ba.md)

    Inserts the specified element to the queue. 

* [iterator insert(const_iterator pos, usize count, const value_type &value)](class_luna_1_1_ring_deque_1a1f971372764eaa00ecb6b7a90f31d1e1.md)

    Inserts several copies of the element to the queue. 

* [auto insert(const_iterator pos, _InputIt first, _InputIt last) -> enable_if_t<!is_integral_v< _InputIt >, iterator >](class_luna_1_1_ring_deque_1a4def82cce5edd6eaf0715925cdd6aa9a.md)

    Inserts one range of elements to the queue. 

* [iterator insert(const_iterator pos, InitializerList< value_type > ilist)](class_luna_1_1_ring_deque_1ae23f912fce8b1988a7a54d4cbcf39c0c.md)

    Inserts one range of elements specified by the initializer list to the queue. 

* [iterator erase(const_iterator pos)](class_luna_1_1_ring_deque_1a29790c28710ec0e64b48c2f4edd0b08c.md)

    Removes one element from the queue. 

* [iterator erase(const_iterator first, const_iterator last)](class_luna_1_1_ring_deque_1aa3af768723cd533218ea3d83af440713.md)

    Removes one range of elements from the queue. 

* [void swap(RingDeque &rhs)](class_luna_1_1_ring_deque_1a7b9a39ce6eac83388670863be401bb3d.md)

    Swaps elements of this queue with the specified queue. 

* [iterator emplace(const_iterator pos, _Args &&... args)](class_luna_1_1_ring_deque_1a5a790d148428f16e8396ebbc1e971c18.md)

    Constructs one element directly on the specified position of the queue using the provided arguments. 

* [iterator emplace_back(_Args &&... args)](class_luna_1_1_ring_deque_1a8548c2ae5f27a168e0793186d997848d.md)

    Constructs one element directly on the back of the queue using the provided arguments. 

* [iterator emplace_front(_Args &&... args)](class_luna_1_1_ring_deque_1a7ad70b775c215d1c93fcf06d8ae9db55.md)

    Constructs one element directly on the front of the queue using the provided arguments. 

* [allocator_type get_allocator() const](class_luna_1_1_ring_deque_1a6e99c6263568d88f95ca01dc694f1051.md)

    Gets the allocator of the queue. 

