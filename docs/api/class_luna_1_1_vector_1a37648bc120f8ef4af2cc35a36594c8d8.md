# Luna::Vector::insert

```c++
template <typename _Rty>
Vector< _Ty, _Alloc >::iterator insert(const_iterator pos, Span< _Rty > data)
```

Inserts elements specified by the span to the vector. Elements in the span will be copy-inserted into the vector. 



## Parameters
* *in* **pos**

    The iterator to the position to insert elements. The elements will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the vector. 

* *in* **data**

    The span that specifies elements to copy from. 

## Return value
Returns one iterator to the inserted element. 

## Valid Usage
* If `pos != end()`, `pos` must points to a valid element in the vector. 

