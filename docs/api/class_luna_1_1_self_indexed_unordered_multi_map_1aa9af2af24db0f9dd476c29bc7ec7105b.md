# Luna::SelfIndexedUnorderedMultiMap::rehash

```c++
void rehash(usize new_buckets_count)
```

Changes the bucket count and rehashes all elements to insert them to the new buckets. 



## Parameters
* *in* **new_buckets_count**

    The new bucket count to set. 

## Remark
If the new bucket count is too small or makes load factor exceed load factor limits, the new bucket count will be expanded to a minimum value that satisfies requirements. You can specify `new_buckets_count` to `0` to shrink the map. 

