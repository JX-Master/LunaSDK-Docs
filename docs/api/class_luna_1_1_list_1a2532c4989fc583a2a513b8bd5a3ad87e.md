# Luna::List::insert

```c++
List< _Ty, _Alloc >::iterator insert(const_iterator pos, usize count, const value_type &value)
```

Inserts several copies of the element to the list. 

## Overview


## Parameters
### pos
The iterator pointing to the position to insert elements. The elements will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the list. 

### count
The number of elements to insert. 

### value
The value to initialize the new elements with. 

## Return value
Returns one iterator pointing to the first inserted element. 

#### Valid Usage
* If `pos != end()`, `pos` must points to a valid element in the list. 

