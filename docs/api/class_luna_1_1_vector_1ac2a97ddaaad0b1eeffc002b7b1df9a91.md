# Luna::Vector::insert

```c++
Vector< _Ty, _Alloc >::iterator insert(const_iterator pos, value_type &&value)
```

Inserts the specified element to the vector. 



## Parameters
* *in* **pos**

    The iterator to the position to insert the element. The element will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the vector. 

* *in* **value**

    The element to insert. The element will be move-inserted into the vector. 

## Return value
Returns one iterator to the inserted element. 

## Valid Usage
* If `pos != end()`, `pos` must points to a valid element in the vector. 

