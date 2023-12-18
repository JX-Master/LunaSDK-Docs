# Luna::find_end

```c++
template <typename _ForwardIt>
auto find_end(_ForwardIt first, _ForwardIt last, _ForwardIt pattern_first, _ForwardIt pattern_last) -> enable_if_t< is_pointer_v< _ForwardIt >, _ForwardIt >
```

Searches for the last occurrence of the sequence of elements in the specified range. 



## Parameters
* *in* **first**

    The iterator to the first element of the search range. 

* *in* **last**

    The iterator to the one-past-last element of the search range. 

* *in* **pattern_first**

    The iterator to the first element of the sequence to search. 

* *in* **pattern_last**

    The iterator to the one-past-last element of the sequence to search. 

## Return value
Returns one iterator to the beginning of last occurrence of the sequence[`pattern_first`, `pattern_last`). Returns `last` if no such occurrence is found. 

