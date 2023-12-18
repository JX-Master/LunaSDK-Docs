# Luna::SelfIndexedUnorderedMap::load_factor

```c++
f32 load_factor() const
```

Gets the load factor of the map, which can be computed by `(f32)size() / (f32)bucket_count()`. 



## Return value
Returns the load factor of the map. Returns `0.0f` if [bucket_count](class_luna_1_1_self_indexed_unordered_map_1ace2cb5dc8f915f78658dac76efacd4c1.md) is `0`. 

