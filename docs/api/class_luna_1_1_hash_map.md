# Luna::HashMap
An container that contains key-value pairs with unique keys using open-addressing hashing algorithm. 

```c++
class Luna::HashMap
```

## Overview

Prefer [HashMap](class_luna_1_1_hash_map.md) and [HashSet](class_luna_1_1_hash_set.md) instead of UnorderedMap and UnorderedSet, since it performs better in memory fragmentation, memory locality and cache performance. Use UnorderedMap and UnorderedSet if you have the following requirements:

## Functions
* [HashMap()](class_luna_1_1_hash_map_1a8e7da885280257b837a2de2b94e02fcd.md)

    Constructs an empty map. 

* [HashMap(const allocator_type &alloc)](class_luna_1_1_hash_map_1a94faee862d13b8063b31b884435eed05.md)

    Constructs an empty map with an custom allocator. 

* [HashMap(const HashMap &rhs)](class_luna_1_1_hash_map_1a78b0dadb3f961dd5f665d295f90f9391.md)

    Constructs a map by coping elements from another map. 

* [HashMap(const HashMap &rhs, const allocator_type &alloc)](class_luna_1_1_hash_map_1a01ee6fafc0882937510946f626f6bc9e.md)

    Constructs a map with an custom allocator and with elements copied from another map. 

* [HashMap(HashMap &&rhs)](class_luna_1_1_hash_map_1ae8fa1ee213412e9dd0bce31f3837a3eb.md)

    Constructs a map by moving elements from another map. 

* [HashMap(HashMap &&rhs, const allocator_type &alloc)](class_luna_1_1_hash_map_1aecfd83a95d996d423d5e746946c27fff.md)

    Constructs a map with an custom allocator and with elements moved from another map. 

* [iterator begin()](class_luna_1_1_hash_map_1ad69bd11391be1a1dba5c8202259664f8.md)

    Gets one iterator pointing to the first element of the map. 

* [const_iterator begin() const](class_luna_1_1_hash_map_1a29305669b60ca1680752e2fc3592ba99.md)

    Gets one constant iterator pointing to the first element of the map. 

* [const_iterator cbegin() const](class_luna_1_1_hash_map_1a39112ae08f6ffc7ee58c6aa79772e094.md)

    Gets one constant iterator pointing to the first element of the map. 

* [iterator end()](class_luna_1_1_hash_map_1acad38d52497a975bfb6f2f6acd76631f.md)

    Gets one iterator pointing to the one past last element of the map. 

* [const_iterator end() const](class_luna_1_1_hash_map_1accf9a4bd0c34d4a5f6a7dab66ea10cdc.md)

    Gets one constant iterator pointing to the one past last element of the map. 

* [const_iterator cend() const](class_luna_1_1_hash_map_1a93791e61ab486b4022c389d634b4facc.md)

    Gets one constant iterator pointing to the one past last element of the map. 

* [bool empty() const](class_luna_1_1_hash_map_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this map is empty, that is, the size of this map is `0`. 

* [usize size() const](class_luna_1_1_hash_map_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the map, that is, the number of elements in the map. 

* [usize capacity() const](class_luna_1_1_hash_map_1ad96bf59cb22e917cbd210ba068e8acb3.md)

    Gets the capacity of the map, that is, the number of elements the hash table can hold before expanding the hash table. 

* [usize hash_table_size() const](class_luna_1_1_hash_map_1ace4cb83fbe1efc093ab5cd0180cc6868.md)

    Gets the hash table size of the map, that is, the number of slots of the hash table array. 

* [f32 load_factor() const](class_luna_1_1_hash_map_1a98c20997abc3070d80e9c2e70afa0493.md)

    Gets the load factor of the map, which can be computed by `(f32)size() / (f32)hash_table_size()`. 

* [f32 max_load_factor() const](class_luna_1_1_hash_map_1aebb6ef2d39e739cc28a67244e423a3a8.md)

    Gets the maximum load factor allowed for the map. 

* [void max_load_factor(f32 ml)](class_luna_1_1_hash_map_1a9102a0c114eea9587ad22afc2a1ccc3c.md)

    Sets the maximum load factor allowed for the map. 

* [void clear()](class_luna_1_1_hash_map_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all elements in the map. 

* [void shrink_to_fit()](class_luna_1_1_hash_map_1a5f16304f80b6fb253c7b0ead3e16dd18.md)

    Reduces the hash table size to a minimum value that satisfy the maximum load factor limitation. 

* [hasher hash_function() const](class_luna_1_1_hash_map_1a72ffe2880da1c06d22d90000f9720967.md)

    Gets the hash function used by this map. 

* [key_equal key_eq() const](class_luna_1_1_hash_map_1a10b2be386447b0ab61e83d0f5527b688.md)

    Gets the equality comparison function used by this map. 

* [void rehash(usize new_data_table_size)](class_luna_1_1_hash_map_1adf0955ccf1cdbb66fd3e51036166efbb.md)

    Changes the data table size and rehashes all elements to insert them to the new data table. 

* [void reserve(usize new_cap)](class_luna_1_1_hash_map_1aa1c32ac6498d3f6d21cab98d1cbf3455.md)

    Expands the data table size to the specified value. 

* [iterator find(const key_type &key)](class_luna_1_1_hash_map_1a9c9766a96c492f3e9e5861d6b4f87387.md)

    Finds the specified element in the map. 

* [const_iterator find(const key_type &key) const](class_luna_1_1_hash_map_1af2a080484f0b756af6f218c0e6bae306.md)

    Finds the specified element in the map. 

* [usize count(const key_type &key) const](class_luna_1_1_hash_map_1a2d5dc5e3872df3149f3c3ac730ff5607.md)

    Gets the number of elements whose key is equal to the specified key. 

* [bool contains(const key_type &key) const](class_luna_1_1_hash_map_1aa0b05f4f6c691fbe71159c631dded53b.md)

    Checks whether at least one element with the specified key exists. 

* [Pair< iterator, bool > insert(const value_type &value)](class_luna_1_1_hash_map_1a45549ac2883165244dbc0005a33dac64.md)

    Inserts the specified key-value pair to the map. 

* [Pair< iterator, bool > insert(value_type &&value)](class_luna_1_1_hash_map_1adfc3632f295d0c500bafbe68b91757f8.md)

    Inserts the specified key-value pair to the map. 

* [Pair< iterator, bool > insert_or_assign(const key_type &key, _M &&value)](class_luna_1_1_hash_map_1aad213718c308bedbbf92cb81e182cf54.md)

    Assigns the value to the element with the specified key, or inserts the key-value pair to the map if such element is not found. 

* [Pair< iterator, bool > insert_or_assign(key_type &&key, _M &&value)](class_luna_1_1_hash_map_1aec69432164a51529a980ba873fbc0c64.md)

    Assigns the value to the element with the specified key, or inserts the key-value pair to the map if such element is not found. 

* [Pair< iterator, bool > emplace(_Args &&... args)](class_luna_1_1_hash_map_1a044dbf1291b7cfaae7c7f433d582f937.md)

    Constructs one element directly in the map using the provided arguments. 

* [iterator erase(const_iterator pos)](class_luna_1_1_hash_map_1a29790c28710ec0e64b48c2f4edd0b08c.md)

    Removes one element from the map. 

* [usize erase(const key_type &key)](class_luna_1_1_hash_map_1a34dd266404ddfcb1683866f0c203904e.md)

    Removes elements with the specified key from the map. 

* [void swap(HashMap &rhs)](class_luna_1_1_hash_map_1ab26678fec10dd0e3974550c754cf0124.md)

    Swaps elements of this map with the specified map. 

* [allocator_type get_allocator() const](class_luna_1_1_hash_map_1a6e99c6263568d88f95ca01dc694f1051.md)

    Gets the allocator used by this map. 
