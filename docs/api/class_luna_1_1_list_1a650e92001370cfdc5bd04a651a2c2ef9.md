# Luna::List::insert

```c++
template <typename _InputIt>
auto insert(const_iterator pos, _InputIt first, _InputIt last) -> enable_if_t<!is_integral_v< _InputIt >, List< _Ty, _Alloc >::iterator >
```

Inserts one range of elements to the list. 



## Parameters
* *in* **pos**

    The iterator pointing to the position to insert elements. The elements will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the list. 

* *in* **first**

    The iterator pointing to the first element to be inserted. 

* *in* **last**

    The iterator pointing to the one-past-last element to be inserted. 

## Return value
Returns one iterator pointing to the first inserted element. 

## Valid Usage
* If `pos != end()`, `pos` must points to a valid element in the list. 

