# Luna::HashSet::max_load_factor

```c++
f32 max_load_factor() const
```

Gets the maximum load factor allowed for the set. 

If `load_factor() > max_load_factor()` is `true` after one element is inserted, the set will expand the hash table to bring more hash table slots. 

## Return value
Returns the maximum load factor allowed for the set. 

