# Luna::List
A container that stores elements as double-linked lists (nodes connected by pointers). 

```c++
class Luna::List
```

## Functions
* [List()](class_luna_1_1_list_1a17e6c90f14225bdac5c65ed915b0a2f6.md)

    Constructs an empty list. 

* [List(const allocator_type &alloc)](class_luna_1_1_list_1ae611567eda6d2e25cf0b551cfe932f1d.md)

    Constructs an empty list with an custom allocator. 

* [List(usize count, const_reference value, const allocator_type &alloc=allocator_type())](class_luna_1_1_list_1a251d138a94e827712a83f49b4cef65a9.md)

    Constructs a list with the specified number of elements. 

* [List(usize count, const allocator_type &alloc=allocator_type())](class_luna_1_1_list_1aa2997a1f0d7569dce584f12f24a0ee7c.md)

    Constructs a list with the specified number of elements. Elements will be default-initialized. 

* [List(enable_if_t<!is_integral_v< _InputIt >, _InputIt > first, _InputIt last, const allocator_type &alloc=allocator_type())](class_luna_1_1_list_1a9013680ffde3a32db98bcee53a4e1499.md)

    Constructs a list with elements specified by one range. Elements in the range will be copy-inserted into the list. 

* [List(const List &rhs)](class_luna_1_1_list_1a7d9a3513b0c4ce2d4a9d380e5046597f.md)

    Constructs a list by copying elements from another list. 

* [List(const List &rhs, const allocator_type &alloc)](class_luna_1_1_list_1adf956d3c1d0d18dbab020d516adb868a.md)

    Constructs a list with an custom allocator and with elements copied from another list. 

* [List(List &&rhs)](class_luna_1_1_list_1a09400e81df2e73cf04d8233bb49d7241.md)

    Constructs a list by moving elements from another list. 

* [List(List &&rhs, const allocator_type &alloc)](class_luna_1_1_list_1abd1f6d5eae1fda09c94e99d624a31efd.md)

    Constructs a list with an custom allocator and with elements moved from another list. 

* [List(InitializerList< value_type > ilist, const allocator_type &alloc=allocator_type())](class_luna_1_1_list_1a5bfd383cd0ac9b1ffb3a506614af208c.md)

    Constructs a list with elements specified by one initializer list. 

* [List< _Ty, _Alloc > & operator=(const List &rhs)](class_luna_1_1_list_1a8f3b26193f01b56297c3c18713ba9ef7.md)

    Replaces elements of the list by coping elements from another list. 

* [List< _Ty, _Alloc > & operator=(List &&rhs)](class_luna_1_1_list_1a273a8d653cc24bdb145322a79408b192.md)

    Replaces elements of the list by moving elements from another list. 

* [List< _Ty, _Alloc > & operator=(InitializerList< value_type > ilist)](class_luna_1_1_list_1a94af6ef06d505162a657a8c2b0496ec0.md)

    Replaces elements of the list by elements from one initializer list. 

* [void assign(usize count, const value_type &value)](class_luna_1_1_list_1aafc1352043c99963fa09825f1a384a10.md)

    Replaces elements of the list by several copies of the specified value. 

* [auto assign(_InputIt first, _InputIt last) -> enable_if_t<!is_integral_v< _InputIt >, void >](class_luna_1_1_list_1adaeab1488f29b931a806d420cf0857e4.md)

    Replaces elements of the list by elements specified by one range. Elements in the range will be copy-inserted into the list. 

* [void assign(InitializerList< value_type > ilist)](class_luna_1_1_list_1af80ee60b2d616a86fe008cf226795f26.md)

    Replaces elements of the list by elements from one initializer list. 

* [List< _Ty, _Alloc >::reference front()](class_luna_1_1_list_1ab224d00c52b43f870e827b15993bc2fe.md)

    Gets the first element in the list. 

* [List< _Ty, _Alloc >::const_reference front() const](class_luna_1_1_list_1aeef1ee04f94a3045a91a3de58b3833b6.md)

    Gets the first element in the list. 

* [List< _Ty, _Alloc >::reference back()](class_luna_1_1_list_1afe76b6d22e154f4d315d4def8ecf31a4.md)

    Gets the last element in the list. 

* [List< _Ty, _Alloc >::const_reference back() const](class_luna_1_1_list_1a28caa17eb291da14069202da4ff70299.md)

    Gets the last element in the list. 

* [List< _Ty, _Alloc >::iterator begin()](class_luna_1_1_list_1ae49b602ba0b25adb8379bf8727507324.md)

    Gets one iterator pointing to the first element of the list. 

* [List< _Ty, _Alloc >::const_iterator begin() const](class_luna_1_1_list_1a520e28135a0b37738c459a2f0c182dff.md)

    Gets one constant iterator pointing to the first element of the list. 

* [List< _Ty, _Alloc >::const_iterator cbegin() const](class_luna_1_1_list_1a75f81254aa74d19c9e72bbe3bdd92c8a.md)

    Gets one constant iterator pointing to the first element of the list. 

* [List< _Ty, _Alloc >::iterator end()](class_luna_1_1_list_1a7ec56631bf0f334d845e6a198618360a.md)

    Gets one iterator pointing to the one past last element of the list. 

* [List< _Ty, _Alloc >::const_iterator end() const](class_luna_1_1_list_1a33e164de8d71f0ce8ddc3d7b8fc567e0.md)

    Gets one constant iterator pointing to the one past last element of the list. 

* [List< _Ty, _Alloc >::const_iterator cend() const](class_luna_1_1_list_1a55c434a81cad9990fb3429a3e549657f.md)

    Gets one constant iterator pointing to the one past last element of the list. 

* [List< _Ty, _Alloc >::reverse_iterator rbegin()](class_luna_1_1_list_1abe03ab15dca2df019aa3b28ae52081d7.md)

    Gets one reverse iterator pointing to the last element of the list. 

* [List< _Ty, _Alloc >::const_reverse_iterator rbegin() const](class_luna_1_1_list_1ae9756b0302b9bea3fc6094fcc773acef.md)

    Gets one constant reverse iterator pointing to the last element of the list. 

* [List< _Ty, _Alloc >::const_reverse_iterator crbegin() const](class_luna_1_1_list_1aa378c7002668de375ecb9b69f0173520.md)

    Gets one constant reverse iterator pointing to the last element of the list. 

* [List< _Ty, _Alloc >::reverse_iterator rend()](class_luna_1_1_list_1a5b16bb5e06bf3ed7733795fab95d9492.md)

    Gets one reverse iterator pointing to the one-before-first element of the list. 

* [List< _Ty, _Alloc >::const_reverse_iterator rend() const](class_luna_1_1_list_1acef94bdef07ba09516830c5d427f7c87.md)

    Gets one constant reverse iterator pointing to the one-before-first element of the list. 

* [List< _Ty, _Alloc >::const_reverse_iterator crend() const](class_luna_1_1_list_1aeeb4338da0a6043328f277d27c783d34.md)

    Gets one constant reverse iterator pointing to the one-before-first element of the list. 

* [bool empty() const](class_luna_1_1_list_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this list is empty, that is, the size of this list is `0`. 

* [usize size() const](class_luna_1_1_list_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the list, that is, the number of elements in the list. 

* [void clear()](class_luna_1_1_list_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all elements in the list. 

* [List< _Ty, _Alloc >::iterator insert(const_iterator pos, const value_type &value)](class_luna_1_1_list_1a99f2047c0b82c7ea135983a5925ad28b.md)

    Inserts the specified element to the list. 

* [List< _Ty, _Alloc >::iterator insert(const_iterator pos, value_type &&value)](class_luna_1_1_list_1a80b6f2d2e03ae9edc8117ade0716e70d.md)

    Inserts the specified element to the list. 

* [List< _Ty, _Alloc >::iterator insert(const_iterator pos, usize count, const value_type &value)](class_luna_1_1_list_1a2532c4989fc583a2a513b8bd5a3ad87e.md)

    Inserts several copies of the element to the list. 

* [auto insert(const_iterator pos, _InputIt first, _InputIt last) -> enable_if_t<!is_integral_v< _InputIt >, List< _Ty, _Alloc >::iterator >](class_luna_1_1_list_1a650e92001370cfdc5bd04a651a2c2ef9.md)

    Inserts one range of elements to the list. 

* [List< _Ty, _Alloc >::iterator insert(const_iterator pos, InitializerList< value_type > ilist)](class_luna_1_1_list_1a6e7b23b089aa694e8076d13dae6bac3d.md)

    Inserts one range of elements specified by the initializer list to the list. 

* [List< _Ty, _Alloc >::iterator emplace(const_iterator pos, _Args &&... args)](class_luna_1_1_list_1a4aa5c144e127e2247b2fcdb6eb769b2b.md)

    Constructs one element directly on the specified position of the list using the provided arguments. 

* [List< _Ty, _Alloc >::iterator erase(const_iterator pos)](class_luna_1_1_list_1a8c7c76ca5168dd917dfbe2cba9a57e60.md)

    Removes one element from the list. 

* [List< _Ty, _Alloc >::iterator erase(const_iterator first, const_iterator last)](class_luna_1_1_list_1a351c85f0e22a5f6ef21aee32a62cfbb5.md)

    Removes one range of elements from the list. 

* [void push_back(const value_type &value)](class_luna_1_1_list_1ab249999c1e6caf5fc15da072edfb7cf2.md)

    Inserts one element at the back of the list. 

* [void push_back(value_type &&value)](class_luna_1_1_list_1adc7b837f89f7e8dddcf2dc276dc115b2.md)

    Inserts one element at the back of the list. 

* [List< _Ty, _Alloc >::reference emplace_back(_Args &&... args)](class_luna_1_1_list_1ab877c1d244ce584e04e71592cc5fb28b.md)

    Constructs one element directly on the back of the list using the provided arguments. 

* [void pop_back()](class_luna_1_1_list_1a058bda4957df6a97b1ea6c9fd783f672.md)

    Removes the last element of the list. 

* [void push_front(const value_type &value)](class_luna_1_1_list_1a318102205e1258cfeff6c5ba6d1ceaf6.md)

    Inserts one element at the front of the list. 

* [void push_front(value_type &&value)](class_luna_1_1_list_1ac5507a062255b274ef3b0557b5925087.md)

    Inserts one element at the front of the list. 

* [List< _Ty, _Alloc >::reference emplace_front(_Args &&... args)](class_luna_1_1_list_1ac80bf569e193eb38de839b1fc2d2b508.md)

    Constructs one element directly on the front of the list using the provided arguments. 

* [void pop_front()](class_luna_1_1_list_1a56f4ffbc6fd414b3c02a6c368e99594f.md)

    Removes the first element of the list. 

* [void resize(usize count)](class_luna_1_1_list_1afe7d58790aad6d1244777711aef39ad0.md)

    Changes the number of elements in the list. 

* [void resize(usize count, const value_type &value)](class_luna_1_1_list_1a05ef093245a3749df69b46f59230454b.md)

    Changes the number of elements in the list. 

* [void swap(List &rhs)](class_luna_1_1_list_1a67991a77c21b55d8a770cd3a8e36cd34.md)

    Swaps elements of this list with the specified list. 

* [void merge(List &other)](class_luna_1_1_list_1aadabb3f9c00e459c78581e00207a9f2f.md)

    Merges another list into this list. 

* [void merge(List &&other)](class_luna_1_1_list_1a92d577d3e25fe2d9e2ab698c461f5189.md)

    Merges another list into this list. 

* [void merge(List &other, _Compare comp)](class_luna_1_1_list_1af2b6dc300d3ff9b1ac3ad178bd4d0b4d.md)

    Merges another list into this list. 

* [void merge(List &&other, _Compare comp)](class_luna_1_1_list_1a2f8f6e82f209f35a4a02e978b03ffea9.md)

    Merges another list into this list. 

* [void splice(const_iterator pos, List &other)](class_luna_1_1_list_1a9e4924c2cff390d0bfe276fd83eb0aa9.md)

    Transfers all elements from another list to this list. 

* [void splice(const_iterator pos, List &&other)](class_luna_1_1_list_1a5553842996c4ac239a5311aad4c29252.md)

    Transfers all elements from another list to this list. 

* [void splice(const_iterator pos, List &other, const_iterator it)](class_luna_1_1_list_1ad7f3db2f149b0faf686e81595f2c333a.md)

    Transfers one element from another list to this list. 

* [void splice(const_iterator pos, List &&other, const_iterator it)](class_luna_1_1_list_1afd0e7fad7eae2aa017ac604c1ed6af5f.md)

    Transfers one element from another list to this list. 

* [void splice(const_iterator pos, List &other, const_iterator first, const_iterator last)](class_luna_1_1_list_1a32274c2c8ee987aadfacdf1fd9c6d31a.md)

    Transfers elements from another list to this list. 

* [void splice(const_iterator pos, List &&other, const_iterator first, const_iterator last)](class_luna_1_1_list_1ab467c6181c9578af00b91c1caa15b7ae.md)

    Transfers elements from another list to this list. 

* [usize remove(const value_type &value)](class_luna_1_1_list_1a42ee9dddf42e7f12f53d596ad4451dcb.md)

    Removes all elements that are equal to value. 

* [usize remove_if(_UnaryPredicate p)](class_luna_1_1_list_1a03d8c556a366c8122ccddfc9c24e6ddc.md)

    Removes all elements for which the specified predicate returns `true`. 

* [void reverse()](class_luna_1_1_list_1a310c0bebc002158f5646a91d60e4dc89.md)

    Reverses the order of the elements in the list. 

* [usize unique()](class_luna_1_1_list_1ad95db96bc0c2ccfb45416ad2590561ef.md)

    Removes all consecutive duplicate elements from the container. 

* [usize unique(_BinaryPredicate p)](class_luna_1_1_list_1a74f6d3924c2755549821dd1e4e1875f9.md)

    Removes all consecutive duplicate elements from the container. 

* [void sort()](class_luna_1_1_list_1a47fdc9eea42b6975cdc835bb2e08810e.md)

    Sorts elements in ascending order. 

* [void sort(_Compare comp)](class_luna_1_1_list_1aa410e59eb5490c3896b76be4d5d418f9.md)

    Sorts elements in using the user-specified comparison function object. 

* [List< _Ty, _Alloc >::allocator_type get_allocator() const](class_luna_1_1_list_1a5d1a6ef108d9c2004e07e8183c716d1b.md)

    Gets the allocator of the list. 

