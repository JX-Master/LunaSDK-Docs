# Luna::UnorderedSet::equal_range

```c++
Pair< iterator, iterator > equal_range(const key_type &key)
```

Gets one pair of iterators specifying one range of elements whose keys are equal to the specified key. 



## Parameters
* *in* **key**

    The key to test. 

## Return value
Returns the element range. 

## Remark
Since this set does not allow inserting multiple elements with the same key, the returned range will contain only one element if the key exists, or empty if the key does not exist. 

