# Luna::List::insert

```c++
List< _Ty, _Alloc >::iterator insert(const_iterator pos, InitializerList< value_type > ilist)
```

Inserts one range of elements specified by the initializer list to the list. 



## Parameters
* *in* **pos**

    The iterator pointing to the position to insert elements. The elements will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the list. 

* *in* **ilist**

    The initializer list. 

## Return value
Returns one iterator pointing to the first inserted element. 

## Valid Usage
* If `pos != end()`, `pos` must points to a valid element in the list. 

