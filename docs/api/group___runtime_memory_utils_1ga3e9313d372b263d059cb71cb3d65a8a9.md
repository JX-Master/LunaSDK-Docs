# Luna::fill_assign_range

```c++
template <typename _Iter1, typename _Ty>
_Iter1 fill_assign_range(_Iter1 first, _Iter1 last, const _Ty &value)
```

Performs copy assignment on each of the object in the range by taking a copy of the provided object. 



## Parameters
### first
An iterator to the first object to be assigned. 

### last
An iterator to one-past-last object to be assigned. 

### value
The object to copy from for each object to be assigned. 

## Return value
Returns an iterator to one-past-last object to be assigned. 

