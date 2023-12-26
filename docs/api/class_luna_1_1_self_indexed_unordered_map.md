# Luna::SelfIndexedUnorderedMap
Represents one self-indexed unordered map whose key can be extracted from the value, so that it does not need to be stored. 

```c++
template <typename _Kty, typename _Ty, typename _ExtractKey, typename _Hash, typename _KeyEqual, typename _Alloc>
class Luna::SelfIndexedUnorderedMap
```

For every value type that the user want to use for self indexed unordered map, the user must define one special structure called "key extractor", and passes the type as the `_ExtractKey` template argument for the map. In this structure, one operator function `const _Kty& operator()(const _Ty& p) const` (or `_Kty operator()(const _Ty& p) const` if the key is computed from value) must be defined to fetch the key of the value.

The user must ensure that the key data member is not changed after the element is inserted to the map and before the element is removed from the map, or the behavior is undefined. 

## Member functions
* [SelfIndexedUnorderedMap()](class_luna_1_1_self_indexed_unordered_map_1a14ba9358d0820f56cca8a2db37b7702a.md)

    Constructs an empty map. 

* [SelfIndexedUnorderedMap(const allocator_type &alloc)](class_luna_1_1_self_indexed_unordered_map_1ad9d9dda20c2ca0836cf356aa6c568dfb.md)

    Constructs an empty map with an custom allocator. 

* [SelfIndexedUnorderedMap(const SelfIndexedUnorderedMap &rhs)](class_luna_1_1_self_indexed_unordered_map_1a9269dbfd4318ae43284fe23b2216120f.md)

    Constructs a map by coping elements from another map. 

* [SelfIndexedUnorderedMap(const SelfIndexedUnorderedMap &rhs, const allocator_type &alloc)](class_luna_1_1_self_indexed_unordered_map_1a7bf1281b448c7edc4309ad25d6c2c29a.md)

    Constructs a map with an custom allocator and with elements copied from another map. 

* [SelfIndexedUnorderedMap(SelfIndexedUnorderedMap &&rhs)](class_luna_1_1_self_indexed_unordered_map_1ad4b4754e8b97e592b7d477b6d7584f05.md)

    Constructs a map by moving elements from another map. 

* [SelfIndexedUnorderedMap(SelfIndexedUnorderedMap &&rhs, const allocator_type &alloc)](class_luna_1_1_self_indexed_unordered_map_1aef137fd3730ba415e7b1ebe300a6ce13.md)

    Constructs a map with an custom allocator and with elements moved from another map. 

* [SelfIndexedUnorderedMap & operator=(const SelfIndexedUnorderedMap &rhs)](class_luna_1_1_self_indexed_unordered_map_1a4664d8039c51f4da8b2980ad4112e54e.md)

    Replaces elements of the map by coping elements from another map. 

* [SelfIndexedUnorderedMap & operator=(SelfIndexedUnorderedMap &&rhs)](class_luna_1_1_self_indexed_unordered_map_1a99c99e5f9f7884178b47c2f496413471.md)

    Replaces elements of the map by moving elements from another map. 

* [iterator begin()](class_luna_1_1_self_indexed_unordered_map_1ad69bd11391be1a1dba5c8202259664f8.md)

    Gets one iterator to the first element of the map. 

* [const_iterator begin() const](class_luna_1_1_self_indexed_unordered_map_1a29305669b60ca1680752e2fc3592ba99.md)

    Gets one constant iterator to the first element of the map. 

* [const_iterator cbegin() const](class_luna_1_1_self_indexed_unordered_map_1a39112ae08f6ffc7ee58c6aa79772e094.md)

    Gets one constant iterator to the first element of the map. 

* [iterator end()](class_luna_1_1_self_indexed_unordered_map_1acad38d52497a975bfb6f2f6acd76631f.md)

    Gets one iterator to the one past last element of the map. 

* [const_iterator end() const](class_luna_1_1_self_indexed_unordered_map_1accf9a4bd0c34d4a5f6a7dab66ea10cdc.md)

    Gets one constant iterator to the one past last element of the map. 

* [const_iterator cend() const](class_luna_1_1_self_indexed_unordered_map_1a93791e61ab486b4022c389d634b4facc.md)

    Gets one constant iterator to the one past last element of the map. 

* [local_iterator begin(usize n)](class_luna_1_1_self_indexed_unordered_map_1a93a8c27892c34625c315914f976d8ad3.md)

    Gets an iterator to the first element of the bucket with specified index. 

* [const_local_iterator begin(usize n) const](class_luna_1_1_self_indexed_unordered_map_1a7c785dfed34436fa185d65a54519e310.md)

    Gets an constant iterator to the first element of the bucket with specified index. 

* [const_local_iterator cbegin(usize n) const](class_luna_1_1_self_indexed_unordered_map_1acc95b83df5c80dd26cd48546ded59e53.md)

    Gets a constant iterator to the first element of the bucket with specified index. 

* [local_iterator end(usize n)](class_luna_1_1_self_indexed_unordered_map_1a6c08ca2f925dec867e11119dc0653667.md)

    Gets an iterator to the one-past-last element of the bucket with specified index. 

* [const_local_iterator end(usize n) const](class_luna_1_1_self_indexed_unordered_map_1a7a8207811f9020c5b35303489c032193.md)

    Gets a constant iterator to the one-past-last element of the bucket with specified index. 

* [const_local_iterator cend(usize n) const](class_luna_1_1_self_indexed_unordered_map_1a4de0b59f7dab8a23fcddee7f6aea3229.md)

    Gets a constant iterator to the one-past-last element of the bucket with specified index. 

* [bool empty() const](class_luna_1_1_self_indexed_unordered_map_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this map is empty, that is, the size of this map is `0`. 

* [usize size() const](class_luna_1_1_self_indexed_unordered_map_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the map, that is, the number of elements in the map. 

* [usize capacity() const](class_luna_1_1_self_indexed_unordered_map_1ad96bf59cb22e917cbd210ba068e8acb3.md)

    Gets the capacity of the map, that is, the number of elements the buckets can hold before expanding the bucket buffer. 

* [usize bucket_count() const](class_luna_1_1_self_indexed_unordered_map_1ace2cb5dc8f915f78658dac76efacd4c1.md)

    Gets the number of buckets of the map. 

* [usize bucket_size(usize n) const](class_luna_1_1_self_indexed_unordered_map_1a509e91a3ee50fd0ce4d2793de3e2e5a4.md)

    Gets the number of elements of the specified bucket. 

* [usize bucket(const key_type &key) const](class_luna_1_1_self_indexed_unordered_map_1a0f8b9f48df6b9e00c5749ceb9e057470.md)

    Gets the index of the bucket that stores the specified key. 

* [f32 load_factor() const](class_luna_1_1_self_indexed_unordered_map_1a98c20997abc3070d80e9c2e70afa0493.md)

    Gets the load factor of the map, which can be computed by `(f32)size() / (f32)bucket_count()`. 

* [f32 max_load_factor() const](class_luna_1_1_self_indexed_unordered_map_1aebb6ef2d39e739cc28a67244e423a3a8.md)

    Gets the maximum load factor allowed for the map. 

* [void max_load_factor(f32 ml)](class_luna_1_1_self_indexed_unordered_map_1a9102a0c114eea9587ad22afc2a1ccc3c.md)

    Sets the maximum load factor allowed for the map. 

* [void clear()](class_luna_1_1_self_indexed_unordered_map_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all elements in the map. 

* [hasher hash_function() const](class_luna_1_1_self_indexed_unordered_map_1a72ffe2880da1c06d22d90000f9720967.md)

    Gets the hash function used by this map. 

* [key_equal key_eq() const](class_luna_1_1_self_indexed_unordered_map_1a10b2be386447b0ab61e83d0f5527b688.md)

    Gets the equality comparison function used by this map. 

* [void rehash(usize new_buckets_count)](class_luna_1_1_self_indexed_unordered_map_1aa9af2af24db0f9dd476c29bc7ec7105b.md)

    Changes the bucket count and rehashes all elements to insert them to the new buckets. 

* [void reserve(usize new_cap)](class_luna_1_1_self_indexed_unordered_map_1aa1c32ac6498d3f6d21cab98d1cbf3455.md)

    Expands the bucket buffer so that it can store at least `new_cap` elements without enpanding the bucket buffer again. 

* [iterator find(const key_type &key)](class_luna_1_1_self_indexed_unordered_map_1a9c9766a96c492f3e9e5861d6b4f87387.md)

    Finds the specified element in the map. 

* [const_iterator find(const key_type &key) const](class_luna_1_1_self_indexed_unordered_map_1af2a080484f0b756af6f218c0e6bae306.md)

    Finds the specified element in the map. 

* [usize count(const key_type &key) const](class_luna_1_1_self_indexed_unordered_map_1a2d5dc5e3872df3149f3c3ac730ff5607.md)

    Gets the number of elements whose key is equal to the specified key. 

* [Pair< iterator, iterator > equal_range(const key_type &key)](class_luna_1_1_self_indexed_unordered_map_1a91e5481e78677a16d94aec74dc5bb307.md)

    Gets one pair of iterators specifying one range of elements whose keys are equal to the specified key. 

* [Pair< const_iterator, const_iterator > equal_range(const key_type &key) const](class_luna_1_1_self_indexed_unordered_map_1a040e6cd9e6ade744edce1117ac4313c0.md)

    Gets one pair of iterators specifying one range of elements whose keys are equal to the specified key. 

* [bool contains(const key_type &key) const](class_luna_1_1_self_indexed_unordered_map_1aa0b05f4f6c691fbe71159c631dded53b.md)

    Checks whether at least one element with the specified key exists. 

* [Pair< iterator, bool > insert(const value_type &value)](class_luna_1_1_self_indexed_unordered_map_1a45549ac2883165244dbc0005a33dac64.md)

    Inserts the specified value to the map. The key is extracted from the value. 

* [Pair< iterator, bool > insert(value_type &&value)](class_luna_1_1_self_indexed_unordered_map_1adfc3632f295d0c500bafbe68b91757f8.md)

    Inserts the specified value to the map. The key is extracted from the value. 

* [insert_return_type insert(node_type &&node)](class_luna_1_1_self_indexed_unordered_map_1a23a924435697eb93c6cb5b1b830e8492.md)

    Inserts one node to the map. 

* [Pair< iterator, bool > insert_or_assign(const value_type &value)](class_luna_1_1_self_indexed_unordered_map_1a2f6f02fdd6a85629ea47ad80af730ad4.md)

    Assigns the value to the element with the specified key, or inserts the value pair to the map if such element is not found. The key is extracted from the value. 

* [Pair< iterator, bool > insert_or_assign(value_type &&value)](class_luna_1_1_self_indexed_unordered_map_1ad57ca7fac1264ef84e39c994cf3eec2c.md)

    Assigns the value to the element with the specified key, or inserts the value pair to the map if such element is not found. The key is extracted from the value. 

* [Pair< iterator, bool > emplace(_Args &&... args)](class_luna_1_1_self_indexed_unordered_map_1a044dbf1291b7cfaae7c7f433d582f937.md)

    Constructs one element directly in the map using the provided arguments. 

* [iterator erase(const_iterator pos)](class_luna_1_1_self_indexed_unordered_map_1a29790c28710ec0e64b48c2f4edd0b08c.md)

    Removes one element from the map. 

* [usize erase(const key_type &key)](class_luna_1_1_self_indexed_unordered_map_1a34dd266404ddfcb1683866f0c203904e.md)

    Removes elements with the specified key from the map. 

* [void swap(SelfIndexedUnorderedMap &rhs)](class_luna_1_1_self_indexed_unordered_map_1a6d71cfd7af963575ea89c16c4f9611d0.md)

    Swaps elements of this map with the specified map. 

* [node_type extract(const_iterator pos)](class_luna_1_1_self_indexed_unordered_map_1afe46988223773995582c14171becaaa0.md)

    Extracts one node from the map, so that it can be inserted to another map without any element copy or move operation. 

* [allocator_type get_allocator() const](class_luna_1_1_self_indexed_unordered_map_1a6e99c6263568d88f95ca01dc694f1051.md)

    Gets the allocator used by this map. 

