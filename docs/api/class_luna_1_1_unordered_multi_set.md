# Luna::UnorderedMultiSet
! An container that contains a set of unique objects using closed-addressing hashing algorithm. This container allows multiple copies of the same value exist in the container. 

```c++
template <typename _Kty, typename _Hash, typename _KeyEqual, typename _Alloc>
class Luna::UnorderedMultiSet
```



## Remark
See remarks of [HashMap](class_luna_1_1_hash_map.md) for details. 

## Member functions
* [UnorderedMultiSet()](class_luna_1_1_unordered_multi_set_1a6bedc4ea0acce2dde704a37c256dbd2a.md)

    Constructs an empty set. 

* [UnorderedMultiSet(const allocator_type &alloc)](class_luna_1_1_unordered_multi_set_1a46a2ad34196e1d0a648cbea552010bc8.md)

    Constructs an empty set with an custom allocator. 

* [UnorderedMultiSet(const UnorderedMultiSet &rhs)](class_luna_1_1_unordered_multi_set_1ae78840f1f32af303f6340496e68c5260.md)

    Constructs a set by coping elements from another set. 

* [UnorderedMultiSet(const UnorderedMultiSet &rhs, const allocator_type &alloc)](class_luna_1_1_unordered_multi_set_1af6b5964382f5ac4a72c5ef49e370a825.md)

    Constructs a set with an custom allocator and with elements copied from another set. 

* [UnorderedMultiSet(UnorderedMultiSet &&rhs)](class_luna_1_1_unordered_multi_set_1a5980110f17d162e1ee1944c061a44d33.md)

    Constructs a set by moving elements from another set. 

* [UnorderedMultiSet(UnorderedMultiSet &&rhs, const allocator_type &alloc)](class_luna_1_1_unordered_multi_set_1afb4893de33a8edc2965b1950244c0e1e.md)

    Constructs a set with an custom allocator and with elements moved from another set. 

* [UnorderedMultiSet & operator=(const UnorderedMultiSet &rhs)](class_luna_1_1_unordered_multi_set_1a60e4216fdc9c33bf3e0ad07e48cf726d.md)

    Replaces elements of the set by coping elements from another set. 

* [UnorderedMultiSet & operator=(UnorderedMultiSet &&rhs)](class_luna_1_1_unordered_multi_set_1a1b32af87c066c8e9a04302dcaf3417c9.md)

    Replaces elements of the set by moving elements from another set. 

* [iterator begin()](class_luna_1_1_unordered_multi_set_1ad69bd11391be1a1dba5c8202259664f8.md)

    Gets one iterator to the first element of the set. 

* [const_iterator begin() const](class_luna_1_1_unordered_multi_set_1a29305669b60ca1680752e2fc3592ba99.md)

    Gets one constant iterator to the first element of the set. 

* [const_iterator cbegin() const](class_luna_1_1_unordered_multi_set_1a39112ae08f6ffc7ee58c6aa79772e094.md)

    Gets one constant iterator to the first element of the set. 

* [iterator end()](class_luna_1_1_unordered_multi_set_1acad38d52497a975bfb6f2f6acd76631f.md)

    Gets one iterator to the one past last element of the set. 

* [const_iterator end() const](class_luna_1_1_unordered_multi_set_1accf9a4bd0c34d4a5f6a7dab66ea10cdc.md)

    Gets one constant iterator to the one past last element of the set. 

* [const_iterator cend() const](class_luna_1_1_unordered_multi_set_1a93791e61ab486b4022c389d634b4facc.md)

    Gets one constant iterator to the one past last element of the set. 

* [local_iterator begin(usize n)](class_luna_1_1_unordered_multi_set_1a93a8c27892c34625c315914f976d8ad3.md)

    Gets an iterator to the first element of the bucket with specified index. 

* [const_local_iterator begin(usize n) const](class_luna_1_1_unordered_multi_set_1a7c785dfed34436fa185d65a54519e310.md)

    Gets an constant iterator to the first element of the bucket with specified index. 

* [const_local_iterator cbegin(usize n) const](class_luna_1_1_unordered_multi_set_1acc95b83df5c80dd26cd48546ded59e53.md)

    Gets a constant iterator to the first element of the bucket with specified index. 

* [local_iterator end(usize n)](class_luna_1_1_unordered_multi_set_1a6c08ca2f925dec867e11119dc0653667.md)

    Gets an iterator to the one-past-last element of the bucket with specified index. 

* [const_local_iterator end(usize n) const](class_luna_1_1_unordered_multi_set_1a7a8207811f9020c5b35303489c032193.md)

    Gets a constant iterator to the one-past-last element of the bucket with specified index. 

* [const_local_iterator cend(usize n) const](class_luna_1_1_unordered_multi_set_1a4de0b59f7dab8a23fcddee7f6aea3229.md)

    Gets a constant iterator to the one-past-last element of the bucket with specified index. 

* [bool empty() const](class_luna_1_1_unordered_multi_set_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this set is empty, that is, the size of this set is `0`. 

* [usize size() const](class_luna_1_1_unordered_multi_set_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the set, that is, the number of elements in the set. 

* [usize capacity() const](class_luna_1_1_unordered_multi_set_1ad96bf59cb22e917cbd210ba068e8acb3.md)

    Gets the capacity of the set, that is, the number of elements the buckets can hold before expanding the bucket buffer. 

* [usize bucket_count() const](class_luna_1_1_unordered_multi_set_1ace2cb5dc8f915f78658dac76efacd4c1.md)

    Gets the number of buckets of the set. 

* [usize bucket_size(usize n) const](class_luna_1_1_unordered_multi_set_1a509e91a3ee50fd0ce4d2793de3e2e5a4.md)

    Gets the number of elements of the specified bucket. 

* [usize bucket(const key_type &key) const](class_luna_1_1_unordered_multi_set_1a0f8b9f48df6b9e00c5749ceb9e057470.md)

    Gets the index of the bucket that stores the specified key. 

* [f32 load_factor() const](class_luna_1_1_unordered_multi_set_1a98c20997abc3070d80e9c2e70afa0493.md)

    Gets the load factor of the set, which can be computed by `(f32)size() / (f32)bucket_count()`. 

* [f32 max_load_factor() const](class_luna_1_1_unordered_multi_set_1aebb6ef2d39e739cc28a67244e423a3a8.md)

    Gets the maximum load factor allowed for the set. 

* [void max_load_factor(f32 ml)](class_luna_1_1_unordered_multi_set_1a9102a0c114eea9587ad22afc2a1ccc3c.md)

    Sets the maximum load factor allowed for the set. 

* [void clear()](class_luna_1_1_unordered_multi_set_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all elements in the set. 

* [hasher hash_function() const](class_luna_1_1_unordered_multi_set_1a72ffe2880da1c06d22d90000f9720967.md)

    Gets the hash function used by this set. 

* [key_equal key_eq() const](class_luna_1_1_unordered_multi_set_1a10b2be386447b0ab61e83d0f5527b688.md)

    Gets the equality comparison function used by this set. 

* [void rehash(usize new_buckets_count)](class_luna_1_1_unordered_multi_set_1aa9af2af24db0f9dd476c29bc7ec7105b.md)

    Changes the bucket count and rehashes all elements to insert them to the new buckets. 

* [void reserve(usize new_cap)](class_luna_1_1_unordered_multi_set_1aa1c32ac6498d3f6d21cab98d1cbf3455.md)

    Expands the bucket buffer so that it can store at least `new_cap` elements without enpanding the bucket buffer again. 

* [iterator find(const key_type &key)](class_luna_1_1_unordered_multi_set_1a9c9766a96c492f3e9e5861d6b4f87387.md)

    Finds the specified element in the set. 

* [const_iterator find(const key_type &key) const](class_luna_1_1_unordered_multi_set_1af2a080484f0b756af6f218c0e6bae306.md)

    Finds the specified element in the set. 

* [usize count(const key_type &key) const](class_luna_1_1_unordered_multi_set_1a2d5dc5e3872df3149f3c3ac730ff5607.md)

    Gets the number of elements whose key is equal to the specified key. 

* [Pair< iterator, iterator > equal_range(const key_type &key)](class_luna_1_1_unordered_multi_set_1a91e5481e78677a16d94aec74dc5bb307.md)

    Gets one pair of iterators specifying one range of elements whose keys are equal to the specified key. 

* [Pair< const_iterator, const_iterator > equal_range(const key_type &key) const](class_luna_1_1_unordered_multi_set_1a040e6cd9e6ade744edce1117ac4313c0.md)

    Gets one pair of iterators specifying one range of elements whose keys are equal to the specified key. 

* [bool contains(const key_type &key) const](class_luna_1_1_unordered_multi_set_1aa0b05f4f6c691fbe71159c631dded53b.md)

    Checks whether at least one element with the specified key exists. 

* [iterator insert(const value_type &value)](class_luna_1_1_unordered_multi_set_1a09359ea445ffe7e3238f260dcccca9f6.md)

    Inserts the specified value to the set. The key is extracted from the value. 

* [iterator insert(value_type &&value)](class_luna_1_1_unordered_multi_set_1a56e34f9188c6607e6d6c444f196c329c.md)

    Inserts the specified value to the set. The key is extracted from the value. 

* [iterator insert(node_type &&node)](class_luna_1_1_unordered_multi_set_1a15ecea28bf398e5a54a66476a232803b.md)

    Inserts one node to the set if the node is not empty. 

* [iterator emplace(_Args &&... args)](class_luna_1_1_unordered_multi_set_1ace009a426963c7bcbe03e4b4cac8bea4.md)

    Constructs one element directly in the set using the provided arguments. 

* [iterator erase(const_iterator pos)](class_luna_1_1_unordered_multi_set_1a29790c28710ec0e64b48c2f4edd0b08c.md)

    Removes one element from the set. 

* [usize erase(const key_type &key)](class_luna_1_1_unordered_multi_set_1a34dd266404ddfcb1683866f0c203904e.md)

    Removes elements with the specified key from the set. 

* [void swap(UnorderedMultiSet &rhs)](class_luna_1_1_unordered_multi_set_1a456785c3ae0278c5e9ae868ed906fa08.md)

    Swaps elements of this set with the specified set. 

* [node_type extract(const_iterator pos)](class_luna_1_1_unordered_multi_set_1afe46988223773995582c14171becaaa0.md)

    Extracts one node from the set, so that it can be inserted to another set without any element copy or move operation. 

* [allocator_type get_allocator() const](class_luna_1_1_unordered_multi_set_1a6e99c6263568d88f95ca01dc694f1051.md)

    Gets the allocator used by this set. 

