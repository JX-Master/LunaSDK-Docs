# Luna::fill_construct_range

```c++
template <typename _Iter1, typename _Ty>
_Iter1 fill_construct_range(_Iter1 first, _Iter1 last, const _Ty &value)
```

Performs copy construct on each of the object in the range by taking a copy of the provided object. 



## Parameters
### first
An iterator to the first object to be constructed. 

### last
An iterator to one-past-last object to be constructed. 

### value
The object to copy from for each object to be constructed. 

## Return value
Returns an iterator to one-past-last object to be constructed. 

