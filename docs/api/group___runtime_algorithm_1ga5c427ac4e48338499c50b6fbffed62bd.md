# Luna::find

```c++
template <typename _InputIt, typename _Ty>
constexpr _InputIt find(_InputIt first, _InputIt last, const _Ty &value)
```

Searches for the first element in the range that is equal to (==) the specified value. 

## Overview


## Parameters
### first
The iterator pointing to the first element of the search range. 

### last
The iterator pointing to the one-past-last element of the search range. 

### value
The value to compare for equality. 

## Return value
Returns one iterator pointing to the first element that is equal to the specified value. Returns `last` if not found. 

