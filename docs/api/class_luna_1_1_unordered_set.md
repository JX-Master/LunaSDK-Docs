# Luna::UnorderedSet
An container that contains a set of unique objects using closed-addressing hashing algorithm. 

```c++
template <typename _Kty, typename _Hash, typename _KeyEqual, typename _Alloc>
class Luna::UnorderedSet
```



## Remark
See remarks of [HashMap](class_luna_1_1_hash_map.md) for details. 

## Member functions
* [UnorderedSet()](class_luna_1_1_unordered_set_1ade6e107a9052659d995de5ffd1930fc7.md)

    Constructs an empty set. 

* [UnorderedSet(const allocator_type &alloc)](class_luna_1_1_unordered_set_1a283c1a723f8e7c4e4196084c0732f661.md)

    Constructs an empty set with an custom allocator. 

* [UnorderedSet(const UnorderedSet &rhs)](class_luna_1_1_unordered_set_1a25aa573dd2c9156725be2603b6e2825f.md)

    Constructs a set by coping elements from another set. 

* [UnorderedSet(const UnorderedSet &rhs, const allocator_type &alloc)](class_luna_1_1_unordered_set_1a53110e90bc6793d554365446cba25d60.md)

    Constructs a set with an custom allocator and with elements copied from another set. 

* [UnorderedSet(UnorderedSet &&rhs)](class_luna_1_1_unordered_set_1ad0691e2313196959fb66c101e8b6ecf8.md)

    Constructs a set by moving elements from another set. 

* [UnorderedSet(UnorderedSet &&rhs, const allocator_type &alloc)](class_luna_1_1_unordered_set_1a6377ae1d245a3984b4d0c4321ff4bfc3.md)

    Constructs a set with an custom allocator and with elements moved from another set. 

* [UnorderedSet & operator=(const UnorderedSet &rhs)](class_luna_1_1_unordered_set_1a59d3e3290203490510a3d48b1b954cb7.md)

    Replaces elements of the set by coping elements from another set. 

* [UnorderedSet & operator=(UnorderedSet &&rhs)](class_luna_1_1_unordered_set_1a99119747d7480356a43b176d9e5cb67e.md)

    Replaces elements of the set by moving elements from another set. 

* [iterator begin()](class_luna_1_1_unordered_set_1ad69bd11391be1a1dba5c8202259664f8.md)

    Gets one iterator to the first element of the set. 

* [const_iterator begin() const](class_luna_1_1_unordered_set_1a29305669b60ca1680752e2fc3592ba99.md)

    Gets one constant iterator to the first element of the set. 

* [const_iterator cbegin() const](class_luna_1_1_unordered_set_1a39112ae08f6ffc7ee58c6aa79772e094.md)

    Gets one constant iterator to the first element of the set. 

* [iterator end()](class_luna_1_1_unordered_set_1acad38d52497a975bfb6f2f6acd76631f.md)

    Gets one iterator to the one past last element of the set. 

* [const_iterator end() const](class_luna_1_1_unordered_set_1accf9a4bd0c34d4a5f6a7dab66ea10cdc.md)

    Gets one constant iterator to the one past last element of the set. 

* [const_iterator cend() const](class_luna_1_1_unordered_set_1a93791e61ab486b4022c389d634b4facc.md)

    Gets one constant iterator to the one past last element of the set. 

* [local_iterator begin(usize n)](class_luna_1_1_unordered_set_1a93a8c27892c34625c315914f976d8ad3.md)

    Gets an iterator to the first element of the bucket with specified index. 

* [const_local_iterator begin(usize n) const](class_luna_1_1_unordered_set_1a7c785dfed34436fa185d65a54519e310.md)

    Gets an constant iterator to the first element of the bucket with specified index. 

* [const_local_iterator cbegin(usize n) const](class_luna_1_1_unordered_set_1acc95b83df5c80dd26cd48546ded59e53.md)

    Gets a constant iterator to the first element of the bucket with specified index. 

* [local_iterator end(usize n)](class_luna_1_1_unordered_set_1a6c08ca2f925dec867e11119dc0653667.md)

    Gets an iterator to the one-past-last element of the bucket with specified index. 

* [const_local_iterator end(usize n) const](class_luna_1_1_unordered_set_1a7a8207811f9020c5b35303489c032193.md)

    Gets a constant iterator to the one-past-last element of the bucket with specified index. 

* [const_local_iterator cend(usize n) const](class_luna_1_1_unordered_set_1a4de0b59f7dab8a23fcddee7f6aea3229.md)

    Gets a constant iterator to the one-past-last element of the bucket with specified index. 

* [bool empty() const](class_luna_1_1_unordered_set_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this set is empty, that is, the size of this set is `0`. 

* [usize size() const](class_luna_1_1_unordered_set_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the set, that is, the number of elements in the set. 

* [usize capacity() const](class_luna_1_1_unordered_set_1ad96bf59cb22e917cbd210ba068e8acb3.md)

    Gets the capacity of the set, that is, the number of elements the hash table can hold before expanding the hash table. 

* [usize bucket_count() const](class_luna_1_1_unordered_set_1ace2cb5dc8f915f78658dac76efacd4c1.md)

    Gets the number of buckets of the set. 

* [usize bucket_size(usize n) const](class_luna_1_1_unordered_set_1a509e91a3ee50fd0ce4d2793de3e2e5a4.md)

    Gets the number of elements of the specified bucket. 

* [usize bucket(const key_type &key) const](class_luna_1_1_unordered_set_1a0f8b9f48df6b9e00c5749ceb9e057470.md)

    Gets the index of the bucket that stores the specified key. 

* [f32 load_factor() const](class_luna_1_1_unordered_set_1a98c20997abc3070d80e9c2e70afa0493.md)

    Gets the load factor of the set, which can be computed by `(f32)size() / (f32)bucket_count()`. 

* [f32 max_load_factor() const](class_luna_1_1_unordered_set_1aebb6ef2d39e739cc28a67244e423a3a8.md)

    Gets the maximum load factor allowed for the set. 

* [void max_load_factor(f32 ml)](class_luna_1_1_unordered_set_1a9102a0c114eea9587ad22afc2a1ccc3c.md)

    Sets the maximum load factor allowed for the set. 

* [void clear()](class_luna_1_1_unordered_set_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all elements in the set. 

* [hasher hash_function() const](class_luna_1_1_unordered_set_1a72ffe2880da1c06d22d90000f9720967.md)

    Gets the hash function used by this set. 

* [key_equal key_eq() const](class_luna_1_1_unordered_set_1a10b2be386447b0ab61e83d0f5527b688.md)

    Gets the equality comparison function used by this set. 

* [void rehash(usize new_buckets_count)](class_luna_1_1_unordered_set_1aa9af2af24db0f9dd476c29bc7ec7105b.md)

    Changes the bucket count and rehashes all elements to insert them to the new buckets. 

* [void reserve(usize new_cap)](class_luna_1_1_unordered_set_1aa1c32ac6498d3f6d21cab98d1cbf3455.md)

    Expands the bucket buffer so that it can store at least `new_cap` elements without enpanding the bucket buffer again. 

* [iterator find(const key_type &key)](class_luna_1_1_unordered_set_1a9c9766a96c492f3e9e5861d6b4f87387.md)

    Finds the specified element in the set. 

* [const_iterator find(const key_type &key) const](class_luna_1_1_unordered_set_1af2a080484f0b756af6f218c0e6bae306.md)

    Finds the specified element in the set. 

* [usize count(const key_type &key) const](class_luna_1_1_unordered_set_1a2d5dc5e3872df3149f3c3ac730ff5607.md)

    Gets the number of elements whose key is equal to the specified key. 

* [Pair< iterator, iterator > equal_range(const key_type &key)](class_luna_1_1_unordered_set_1a91e5481e78677a16d94aec74dc5bb307.md)

    Gets one pair of iterators specifying one range of elements whose keys are equal to the specified key. 

* [Pair< const_iterator, const_iterator > equal_range(const key_type &key) const](class_luna_1_1_unordered_set_1a040e6cd9e6ade744edce1117ac4313c0.md)

    Gets one pair of iterators specifying one range of elements whose keys are equal to the specified key. 

* [bool contains(const key_type &key) const](class_luna_1_1_unordered_set_1aa0b05f4f6c691fbe71159c631dded53b.md)

    Checks whether at least one element with the specified key exists. 

* [Pair< iterator, bool > insert(const value_type &value)](class_luna_1_1_unordered_set_1a45549ac2883165244dbc0005a33dac64.md)

    Inserts the specified value to the set. The key is extracted from the value. 

* [Pair< iterator, bool > insert(value_type &&value)](class_luna_1_1_unordered_set_1adfc3632f295d0c500bafbe68b91757f8.md)

    Inserts the specified value to the set. The key is extracted from the value. 

* [insert_return_type insert(node_type &&node)](class_luna_1_1_unordered_set_1a23a924435697eb93c6cb5b1b830e8492.md)

    Inserts one node to the set. 

* [Pair< iterator, bool > insert_or_assign(const key_type &key, _M &&value)](class_luna_1_1_unordered_set_1aad213718c308bedbbf92cb81e182cf54.md)

    Assigns the value to the element with the specified key, or inserts the value pair to the set if such element is not found. The key is extracted from the value. 

* [Pair< iterator, bool > insert_or_assign(key_type &&key, _M &&value)](class_luna_1_1_unordered_set_1aec69432164a51529a980ba873fbc0c64.md)

    Assigns the value to the element with the specified key, or inserts the value pair to the set if such element is not found. The key is extracted from the value. 

* [Pair< iterator, bool > emplace(_Args &&... args)](class_luna_1_1_unordered_set_1a044dbf1291b7cfaae7c7f433d582f937.md)

    Constructs one element directly in the set using the provided arguments. 

* [iterator erase(const_iterator pos)](class_luna_1_1_unordered_set_1a29790c28710ec0e64b48c2f4edd0b08c.md)

    Removes one element from the set. 

* [usize erase(const key_type &key)](class_luna_1_1_unordered_set_1a34dd266404ddfcb1683866f0c203904e.md)

    Removes elements with the specified key from the set. 

* [void swap(UnorderedSet &rhs)](class_luna_1_1_unordered_set_1a1a8618be0614081d7c10a2e7eeaec9ce.md)

    Swaps elements of this set with the specified set. 

* [node_type extract(const_iterator pos)](class_luna_1_1_unordered_set_1afe46988223773995582c14171becaaa0.md)

    Extracts one node from the set, so that it can be inserted to another set without any element copy or move operation. 

* [allocator_type get_allocator() const](class_luna_1_1_unordered_set_1a6e99c6263568d88f95ca01dc694f1051.md)

    Gets the allocator used by this set. 

