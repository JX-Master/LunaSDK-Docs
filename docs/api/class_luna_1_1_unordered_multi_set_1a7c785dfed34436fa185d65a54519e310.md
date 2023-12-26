# Luna::UnorderedMultiSet::begin

```c++
const_local_iterator begin(usize n) const
```

Gets an constant iterator to the first element of the bucket with specified index. 



## Parameters
* *in* **n**

    The index of the bucket. 

## Return value
Returns one constant iterator to the first element of the bucket. 

## Valid Usage
* `n` must be smaller than [bucket_count](class_luna_1_1_unordered_multi_set_1ace2cb5dc8f915f78658dac76efacd4c1.md). 

