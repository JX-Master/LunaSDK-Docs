# Luna::RingDeque::insert

```c++
iterator insert(const_iterator pos, const value_type &value)
```

Inserts the specified element to the queue. 



## Parameters
* *in* **pos**

    The iterator to the position to insert the element. The element will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the queue. 

* *in* **value**

    The element to insert. The element will be copy-inserted into the queue. 

## Return value
Returns one iterator to the inserted element. 

## Valid Usage
* If `pos != end()`, `pos` must points to a valid element in the queue. 

