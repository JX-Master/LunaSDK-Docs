# Luna::UnorderedMap::extract

```c++
node_type extract(const_iterator pos)
```

Extracts one node from the map, so that it can be inserted to another map without any element copy or move operation. 



## Parameters
* *in* **pos**

    The iterator to the element to be extracted. 

## Return value
Returns the extracted node. 

## Valid Usage
* `pos` must points to a valid element in the map. 

