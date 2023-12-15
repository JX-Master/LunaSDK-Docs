# Luna::List::erase

```c++
List< _Ty, _Alloc >::iterator erase(const_iterator first, const_iterator last)
```

Removes one range of elements from the list. 

## Overview


## Parameters
### first
The iterator pointing to the first element to be removed. 

### last
The iterator pointing to the one-past-last element to be removed. 

## Return value
Returns one iterator pointing to the next element of the removed elements when iterating elements. 

#### Valid Usage
* `first` must be either `end()` or one valid element in the list.

* If `first != end()`, [`first`, `last`) must specifies either one empty range (`first == last`) or one valid element range of the list.

* If `first == end()`, [`first`, `last`) must specifies one empty range (`first == last`). 

