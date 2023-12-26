# Luna::UnorderedMultiSet::insert

```c++
iterator insert(node_type &&node)
```

Inserts one node to the set if the node is not empty. 



## Parameters
* *in* **node**

    The node to insert. The node must be extracted from one unordered set of the same type using [extract](class_luna_1_1_unordered_multi_set_1afe46988223773995582c14171becaaa0.md). 

## Return value
Returns one iterator to the inserted element. Returns `end()` if `node` is empty. 

