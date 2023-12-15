# Luna::search

```c++
template <typename _ForwardIt>
auto search(_ForwardIt first, _ForwardIt last, _ForwardIt pattern_first, _ForwardIt pattern_last) -> enable_if_t< is_pointer_v< _ForwardIt >, _ForwardIt >
```

Searches for the first occurrence of the sequence of elements in the specified range. 

## Overview


## Parameters
### first
The iterator pointing to the first element of the search range. 

### last
The iterator pointing to the one-past-last element of the search range. 

### pattern_first
The iterator pointing to the first element of the sequence to search. 

### pattern_last
The iterator pointing to the one-past-last element of the sequence to search. 

## Return value
Returns one iterator pointing to the beginning of first occurrence of the sequence[`pattern_first`, `pattern_last`). Returns `last` if no such occurrence is found. 

