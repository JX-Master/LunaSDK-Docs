# Luna::sort

```c++
template <typename _RandomIt, typename _Compare>
void sort(_RandomIt first, _RandomIt last, _Compare comp)
```

Sorts the elements in the range in non-descending order. The order of equal elements is not guaranteed to be preserved. 

## Overview


## Parameters
### first
The iterator pointing to the first element of the range. 

### last
The iterator pointing to the one-past-last element of the range. 

### comp
The user-defined comparision function object, which returns `true` if the first argument is less than the second. 

#### Valid Usage
* `comp` must have the following function signature: `bool comp(const Type& a, const Type& b)`, where `Type` is the value type of `_RandomIt`. 

