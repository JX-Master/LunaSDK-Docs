# Luna::OpenHashTable::InsertResult
Represents the insertion result of one node. 

```c++
struct Luna::OpenHashTable::InsertResult
```

## Member objects
* [_Iter position](struct_luna_1_1_open_hash_table_1_1_insert_result_1a07d72ed16c963966df580432fc7e28a5.md)

    The iterator identifing the insertion position if `inserted` is `true`, or. 

* [bool inserted](struct_luna_1_1_open_hash_table_1_1_insert_result_1a325385b8d6787835cb03a2f364ab2c56.md)

    `true` if the insertion is succeeded. `false` if the insertion is failed. 

* [_Node node](struct_luna_1_1_open_hash_table_1_1_insert_result_1a4ce01a83dcdae0ec226d5f4398c0c755.md)

    The original node passed in if the insertion is failed. An empty node otherwise. 

