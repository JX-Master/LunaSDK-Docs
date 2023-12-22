# Luna::UnorderedMultiMap
An container that contains key-value pairs using closed-addressing hashing algorithm. This container allows multiple values with the same key exist in the container. 

```c++
class Luna::UnorderedMultiMap
```



## Remark
See remarks of [HashMap](class_luna_1_1_hash_map.md) for details. 

## Member functions
* [UnorderedMultiMap()](class_luna_1_1_unordered_multi_map_1a458d2beb0d03227554d20ac37d4e2a55.md)

    Constructs an empty map. 

* [UnorderedMultiMap(const allocator_type &alloc)](class_luna_1_1_unordered_multi_map_1a7fa178e3d6f9479246a297749629da14.md)

    Constructs an empty map with an custom allocator. 

* [UnorderedMultiMap(const UnorderedMultiMap &rhs)](class_luna_1_1_unordered_multi_map_1a609c189cdd102dd6f2fdfc64bf1611dd.md)

    Constructs a map by coping elements from another map. 

* [UnorderedMultiMap(const UnorderedMultiMap &rhs, const allocator_type &alloc)](class_luna_1_1_unordered_multi_map_1a2ef804c7f6c35664e5ea8d5750c7aab4.md)

    Constructs a map with an custom allocator and with elements copied from another map. 

* [UnorderedMultiMap(UnorderedMultiMap &&rhs)](class_luna_1_1_unordered_multi_map_1ac4eb3ac6b6ffb5c305ccf72659ab186b.md)

    Constructs a map by moving elements from another map. 

* [UnorderedMultiMap(UnorderedMultiMap &&rhs, const allocator_type &alloc)](class_luna_1_1_unordered_multi_map_1adb8d883389d2c76e312d3ec97bc1d419.md)

    Constructs a map with an custom allocator and with elements moved from another map. 

* [UnorderedMultiMap & operator=(const UnorderedMultiMap &rhs)](class_luna_1_1_unordered_multi_map_1a29f2ac4453206690f0d6142600ce9938.md)

    Replaces elements of the map by coping elements from another map. 

* [UnorderedMultiMap & operator=(UnorderedMultiMap &&rhs)](class_luna_1_1_unordered_multi_map_1a5804619b05010c69d5d0e0edbff19182.md)

    Replaces elements of the map by moving elements from another map. 

* [iterator begin()](class_luna_1_1_unordered_multi_map_1ad69bd11391be1a1dba5c8202259664f8.md)

    Gets one iterator to the first element of the map. 

* [const_iterator begin() const](class_luna_1_1_unordered_multi_map_1a29305669b60ca1680752e2fc3592ba99.md)

    Gets one constant iterator to the first element of the map. 

* [const_iterator cbegin() const](class_luna_1_1_unordered_multi_map_1a39112ae08f6ffc7ee58c6aa79772e094.md)

    Gets one constant iterator to the first element of the map. 

* [iterator end()](class_luna_1_1_unordered_multi_map_1acad38d52497a975bfb6f2f6acd76631f.md)

    Gets one iterator to the one past last element of the map. 

* [const_iterator end() const](class_luna_1_1_unordered_multi_map_1accf9a4bd0c34d4a5f6a7dab66ea10cdc.md)

    Gets one constant iterator to the one past last element of the map. 

* [const_iterator cend() const](class_luna_1_1_unordered_multi_map_1a93791e61ab486b4022c389d634b4facc.md)

    Gets one constant iterator to the one past last element of the map. 

* [local_iterator begin(usize n)](class_luna_1_1_unordered_multi_map_1a93a8c27892c34625c315914f976d8ad3.md)

    Gets an iterator to the first element of the bucket with specified index. 

* [const_local_iterator begin(usize n) const](class_luna_1_1_unordered_multi_map_1a7c785dfed34436fa185d65a54519e310.md)

    Gets an constant iterator to the first element of the bucket with specified index. 

* [const_local_iterator cbegin(usize n) const](class_luna_1_1_unordered_multi_map_1acc95b83df5c80dd26cd48546ded59e53.md)

    Gets a constant iterator to the first element of the bucket with specified index. 

* [local_iterator end(usize n)](class_luna_1_1_unordered_multi_map_1a6c08ca2f925dec867e11119dc0653667.md)

    Gets an iterator to the one-past-last element of the bucket with specified index. 

* [const_local_iterator end(usize n) const](class_luna_1_1_unordered_multi_map_1a7a8207811f9020c5b35303489c032193.md)

    Gets a constant iterator to the one-past-last element of the bucket with specified index. 

* [const_local_iterator cend(usize n) const](class_luna_1_1_unordered_multi_map_1a4de0b59f7dab8a23fcddee7f6aea3229.md)

    Gets a constant iterator to the one-past-last element of the bucket with specified index. 

* [bool empty() const](class_luna_1_1_unordered_multi_map_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this map is empty, that is, the size of this map is `0`. 

* [usize size() const](class_luna_1_1_unordered_multi_map_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the map, that is, the number of elements in the map. 

* [usize capacity() const](class_luna_1_1_unordered_multi_map_1ad96bf59cb22e917cbd210ba068e8acb3.md)

    Gets the capacity of the map, that is, the number of elements the buckets can hold before expanding the bucket buffer. 

* [usize bucket_count() const](class_luna_1_1_unordered_multi_map_1ace2cb5dc8f915f78658dac76efacd4c1.md)

    Gets the number of buckets of the map. 

* [usize bucket_size(usize n) const](class_luna_1_1_unordered_multi_map_1a509e91a3ee50fd0ce4d2793de3e2e5a4.md)

    Gets the number of elements of the specified bucket. 

* [usize bucket(const key_type &key) const](class_luna_1_1_unordered_multi_map_1a0f8b9f48df6b9e00c5749ceb9e057470.md)

    Gets the index of the bucket that stores the specified key. 

* [f32 load_factor() const](class_luna_1_1_unordered_multi_map_1a98c20997abc3070d80e9c2e70afa0493.md)

    Gets the load factor of the map, which can be computed by `(f32)size() / (f32)bucket_count()`. 

* [f32 max_load_factor() const](class_luna_1_1_unordered_multi_map_1aebb6ef2d39e739cc28a67244e423a3a8.md)

    Gets the maximum load factor allowed for the map. 

* [void max_load_factor(f32 ml)](class_luna_1_1_unordered_multi_map_1a9102a0c114eea9587ad22afc2a1ccc3c.md)

    Sets the maximum load factor allowed for the map. 

* [void clear()](class_luna_1_1_unordered_multi_map_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all elements in the map. 

* [hasher hash_function() const](class_luna_1_1_unordered_multi_map_1a72ffe2880da1c06d22d90000f9720967.md)

    Gets the hash function used by this map. 

* [key_equal key_eq() const](class_luna_1_1_unordered_multi_map_1a10b2be386447b0ab61e83d0f5527b688.md)

    Gets the equality comparison function used by this map. 

* [void rehash(usize new_buckets_count)](class_luna_1_1_unordered_multi_map_1aa9af2af24db0f9dd476c29bc7ec7105b.md)

    Changes the bucket count and rehashes all elements to insert them to the new buckets. 

* [void reserve(usize new_cap)](class_luna_1_1_unordered_multi_map_1aa1c32ac6498d3f6d21cab98d1cbf3455.md)

    Expands the bucket buffer so that it can store at least `new_cap` elements without enpanding the bucket buffer again. 

* [iterator find(const key_type &key)](class_luna_1_1_unordered_multi_map_1a9c9766a96c492f3e9e5861d6b4f87387.md)

    Finds the specified element in the map. 

* [const_iterator find(const key_type &key) const](class_luna_1_1_unordered_multi_map_1af2a080484f0b756af6f218c0e6bae306.md)

    Finds the specified element in the map. 

* [usize count(const key_type &key) const](class_luna_1_1_unordered_multi_map_1a2d5dc5e3872df3149f3c3ac730ff5607.md)

    Gets the number of elements whose key is equal to the specified key. 

* [Pair< iterator, iterator > equal_range(const key_type &key)](class_luna_1_1_unordered_multi_map_1a91e5481e78677a16d94aec74dc5bb307.md)

    Gets one pair of iterators specifying one range of elements whose keys are equal to the specified key. 

* [Pair< const_iterator, const_iterator > equal_range(const key_type &key) const](class_luna_1_1_unordered_multi_map_1a040e6cd9e6ade744edce1117ac4313c0.md)

    Gets one pair of iterators specifying one range of elements whose keys are equal to the specified key. 

* [bool contains(const key_type &key) const](class_luna_1_1_unordered_multi_map_1aa0b05f4f6c691fbe71159c631dded53b.md)

    Checks whether at least one element with the specified key exists. 

* [iterator insert(const value_type &value)](class_luna_1_1_unordered_multi_map_1a09359ea445ffe7e3238f260dcccca9f6.md)

    Inserts the specified value to the map. The key is extracted from the value. 

* [iterator insert(value_type &&value)](class_luna_1_1_unordered_multi_map_1a56e34f9188c6607e6d6c444f196c329c.md)

    Inserts the specified value to the map. The key is extracted from the value. 

* [iterator insert(node_type &&node)](class_luna_1_1_unordered_multi_map_1a15ecea28bf398e5a54a66476a232803b.md)

    Inserts one node to the map if the node is not empty. 

* [iterator emplace(_Args &&... args)](class_luna_1_1_unordered_multi_map_1ace009a426963c7bcbe03e4b4cac8bea4.md)

    Constructs one element directly in the map using the provided arguments. 

* [iterator erase(const_iterator pos)](class_luna_1_1_unordered_multi_map_1a29790c28710ec0e64b48c2f4edd0b08c.md)

    Removes one element from the map. 

* [usize erase(const key_type &key)](class_luna_1_1_unordered_multi_map_1a34dd266404ddfcb1683866f0c203904e.md)

    Removes elements with the specified key from the map. 

* [void swap(UnorderedMultiMap &rhs)](class_luna_1_1_unordered_multi_map_1a80ae0d68379b126d91a74b0c0adcd8d9.md)

    Swaps elements of this map with the specified map. 

* [node_type extract(const_iterator pos)](class_luna_1_1_unordered_multi_map_1afe46988223773995582c14171becaaa0.md)

    Extracts one node from the map, so that it can be inserted to another map without any element copy or move operation. 

* [allocator_type get_allocator() const](class_luna_1_1_unordered_multi_map_1a6e99c6263568d88f95ca01dc694f1051.md)

    Gets the allocator used by this map. 

