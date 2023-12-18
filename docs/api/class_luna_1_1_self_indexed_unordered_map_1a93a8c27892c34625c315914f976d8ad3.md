# Luna::SelfIndexedUnorderedMap::begin

```c++
local_iterator begin(usize n)
```

Gets an iterator to the first element of the bucket with specified index. 



## Parameters
* *in* **n**

    The index of the bucket. 

## Return value
Returns one iterator to the first element of the bucket. 

## Valid Usage
* `n` must be smaller than [bucket_count](class_luna_1_1_self_indexed_unordered_map_1ace2cb5dc8f915f78658dac76efacd4c1.md). 

