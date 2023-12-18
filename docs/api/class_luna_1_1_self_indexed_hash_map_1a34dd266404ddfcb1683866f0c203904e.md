# Luna::SelfIndexedHashMap::erase

```c++
usize erase(const key_type &key)
```

Removes elements with the specified key from the map. 



## Parameters
* *in* **key**

    The key of the elements to remove. 

## Return value
Returns the number of elements removed by this operation. 

## Remark
The returned value can only be `0` or `1` for this map type. 

