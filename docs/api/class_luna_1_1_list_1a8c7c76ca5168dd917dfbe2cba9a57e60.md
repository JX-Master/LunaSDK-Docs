# Luna::List::erase

```c++
List< _Ty, _Alloc >::iterator erase(const_iterator pos)
```

Removes one element from the list. 



## Parameters
* *in* **pos**

    The iterator pointing to the element to be removed. 

## Return value
Returns one iterator pointing to the next element of the removed element when iterating elements. 

## Valid Usage
* `pos` must points to a valid element in the list. 

