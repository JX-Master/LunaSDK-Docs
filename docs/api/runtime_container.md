# Containers
## Types
* [Luna::Array](class_luna_1_1_array.md)

    Represents one array of fixed or dynamic size. 


* [Luna::HashMap](class_luna_1_1_hash_map.md)

    An container that contains key-value pairs with unique keys using open-addressing hashing algorithm. 


* [Luna::HashSet](class_luna_1_1_hash_set.md)

    An container that contains a set of unique objects using open-addressing hashing algorithm. 


* [Luna::List](class_luna_1_1_list.md)

    A container that stores elements as double-linked lists (nodes connected by pointers). 


* [Luna::RingDeque](class_luna_1_1_ring_deque.md)

    A container that implements a double-ended queue and uses a ring buffer as its internal storage. 


* [Luna::SelfIndexedHashMap](class_luna_1_1_self_indexed_hash_map.md)

    Represents one self-indexed hash map whose key can be extracted from the value, so that it does not need to be stored. 


* [Luna::SelfIndexedUnorderedMap](class_luna_1_1_self_indexed_unordered_map.md)

    Represents one self-indexed unordered map whose key can be extracted from the value, so that it does not need to be stored. 


* [Luna::SelfIndexedUnorderedMultiMap](class_luna_1_1_self_indexed_unordered_multi_map.md)

    Represents one self-indexed unordered map similar to [SelfIndexedUnorderedMap](class_luna_1_1_self_indexed_unordered_map.md), but allows multiple elements with the same key to be inserted. 


* [Luna::UnorderedMap](class_luna_1_1_unordered_map.md)

    An container that contains key-value pairs with unique keys using closed-addressing hashing algorithm. 


* [Luna::UnorderedMultiMap](class_luna_1_1_unordered_multi_map.md)

    An container that contains key-value pairs using closed-addressing hashing algorithm. This container allows multiple values with the same key exist in the container. 


* [Luna::UnorderedMultiSet](class_luna_1_1_unordered_multi_set.md)

    ! An container that contains a set of unique objects using closed-addressing hashing algorithm. This container allows multiple copies of the same value exist in the container. 


* [Luna::UnorderedSet](class_luna_1_1_unordered_set.md)

    An container that contains a set of unique objects using closed-addressing hashing algorithm. 


* [Luna::Vector](class_luna_1_1_vector.md)

    A container that stores a continuous array of elements. Elements can be added to or removed from the container dynamically. 


## Constants
* [constexpr usize DYNAMIC_ARRAY_SIZE](group___runtime_container_1gac211fb2fcac88253a56c67d77c041a02.md)

    Specifies a dynamic-sized array for [Array](class_luna_1_1_array.md). 

## Functions
* [typeinfo_t hash_map_type()](group___runtime_container_1ga1d3057e6d50ac9a9463512b59e3d8a6f.md)

    Gets the type object of [HashMap](class_luna_1_1_hash_map.md). 

* [typeinfo_t hash_set_type()](group___runtime_container_1ga743bdc5ea347716089749522959567a2.md)

    Gets the type object of [HashSet](class_luna_1_1_hash_set.md). 

* [typeinfo_t vector_type()](group___runtime_container_1ga180f1324922affe17ebe31e278a4716a.md)

    Gets the type object of [Vector](class_luna_1_1_vector.md). 

