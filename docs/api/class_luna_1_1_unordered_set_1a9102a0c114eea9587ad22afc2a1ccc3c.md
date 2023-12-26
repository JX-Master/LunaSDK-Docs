# Luna::UnorderedSet::max_load_factor

```c++
void max_load_factor(f32 ml)
```

Sets the maximum load factor allowed for the set. 

If the new load factor is smaller than `load_factor()`, the set will expand bucket buffer to bring more buckets. 

## Parameters
* *in* **ml**

    The new load factor to set. 

## Valid Usage
* `m` must be greater than `0.0f`. 

