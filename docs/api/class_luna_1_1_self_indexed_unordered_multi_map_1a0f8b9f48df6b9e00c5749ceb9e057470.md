# Luna::SelfIndexedUnorderedMultiMap::bucket

```c++
usize bucket(const key_type &key) const
```

Gets the index of the bucket that stores the specified key. 



## Parameters
* *in* **key**

    The key to check. 

## Return value
Returns the index of the bucket that stores the specified key. 

## Valid Usage
* [bucket_count](class_luna_1_1_self_indexed_unordered_multi_map_1ace2cb5dc8f915f78658dac76efacd4c1.md) must not be `0` when calling this function. 

