# Luna::SelfIndexedHashMap::max_load_factor

```c++
void max_load_factor(f32 ml)
```

Sets the maximum load factor allowed for the map. 

If the new load factor is smaller than `load_factor()`, the map will expand the hash table to bring more hash table slots. 

## Parameters
* *in* **ml**

    The new load factor to set. 

## Valid Usage
* `ml` must between [`0.0`, `1.0`]. 

