# Luna::SelfIndexedUnorderedMap::insert

```c++
insert_return_type insert(node_type &&node)
```

Inserts one node to the map. 



## Parameters
* *in* **node**

    The node to insert. The node must be extracted from one unordered map of the same type using [extract](class_luna_1_1_self_indexed_unordered_map_1afe46988223773995582c14171becaaa0.md). 

## Return value
Returns one structure identifying the insertion result:1. If `node` is empty, `inserted` is false, `position` is `end()`, and `node` is empty.

1. Otherwise if the insertion took place, `inserted` is `true`, `position` points to the inserted element, and `node` is empty.

1. If the insertion failed, `inserted` is false, `node` has the previous value of `node`, and `position` points to an element with a key equivalent to the key of the node. 

