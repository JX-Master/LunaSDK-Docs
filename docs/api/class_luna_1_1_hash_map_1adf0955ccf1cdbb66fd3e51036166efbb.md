# Luna::HashMap::rehash

```c++
void rehash(usize new_data_table_size)
```

Changes the data table size and rehashes all elements to insert them to the new data table. 



## Parameters
* *in* **new_data_table_size**

    The new data table size to set. 

## Remark
If the new data table size is too small or makes load factor exceed load factor limits, the new data table size will be expanded to a minimum value that satisfies requirements. 

