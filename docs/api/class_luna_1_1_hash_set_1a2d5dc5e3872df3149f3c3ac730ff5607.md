# Luna::HashSet::count

```c++
usize count(const key_type &key) const
```

Gets the number of elements whose key is equal to the specified key. 



## Parameters
* *in* **key**

    The key of the element to count. 

## Return value
Returns the number of elements whose key is equal to the specified key. 

## Remark
Since this set does not allow inserting multiple elements with the same key, the returned value will only be `1` if the key exists, or `0` if the key does not exist. 

