# Luna::UnorderedMultiMap::cend

```c++
const_local_iterator cend(usize n) const
```

Gets a constant iterator to the one-past-last element of the bucket with specified index. 



## Parameters
* *in* **n**

    The index of the bucket. 

## Return value
Returns one iterator to the one-past-last element of the bucket. 

## Valid Usage
* `n` must be smaller than [bucket_count](class_luna_1_1_unordered_multi_map_1ace2cb5dc8f915f78658dac76efacd4c1.md). 

