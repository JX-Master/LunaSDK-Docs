# Luna::List::merge

```c++
template <typename _Compare>
void merge(List &other, _Compare comp)
```

Merges another list into this list. 

## Overview
No memory allocation or element copy/move will be performed, this function transfers elements by changing their pointers directly so that they link to the new list. Elements are compared using the user-specified comparison function object. 

## Parameters
### other
The list to merge. This list will be empty after this operation. If this is equal to `*this`, this function does nothing. 

### comp
The comparison function object to use. 

#### Valid Usage
* `comp` must provide the following function: `bool operator()(const _Ty& a, const _Ty& b)`, that returns `true` if `a` should appear in the list before `b`.

* Elements in `*this` and `other` must be sorted in an order defined by the user-specified comparison function, that is, for any two elements `a` and `b` in the same list, `comp(b, a)` must return `false` if `a` appears before `b`. 

