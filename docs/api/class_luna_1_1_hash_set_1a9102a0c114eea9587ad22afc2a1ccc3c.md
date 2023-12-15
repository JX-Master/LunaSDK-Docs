# Luna::HashSet::max_load_factor

```c++
void max_load_factor(f32 ml)
```

Sets the maximum load factor allowed for the set. 

If the new load factor is smaller than `load_factor()`, the set will expand the hash table to bring more hash table slots. 

## Parameters
### ml
The new load factor to set. 

#### Valid Usage
* `ml` must between [`0.0`, `1.0`]. 

