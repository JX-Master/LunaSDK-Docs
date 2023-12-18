# Luna::SelfIndexedHashMap::shrink_to_fit

```c++
void shrink_to_fit()
```

Reduces the hash table size to a minimum value that satisfy the maximum load factor limitation. 

The hash table size can be computed as: `ceilf((f32)size() / max_load_factor())`. 

