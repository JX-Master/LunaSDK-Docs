# Luna::SelfIndexedUnorderedMultiMap::max_load_factor

```c++
f32 max_load_factor() const
```

Gets the maximum load factor allowed for the map. 

If `load_factor() > max_load_factor()` is `true` after one element is inserted, the map will expand bucket buffer to bring more buckets. 

## Return value
Returns the maximum load factor allowed for the map. 

