# Luna::RingDeque::insert

```c++
iterator insert(const_iterator pos, usize count, const value_type &value)
```

Inserts several copies of the element to the queue. 



## Parameters
* *in* **pos**

    The iterator to the position to insert elements. The elements will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the queue. 

* *in* **count**

    The number of elements to insert. 

* *in* **value**

    The value to initialize the new elements with. 

## Return value
Returns one iterator to the first inserted element. 

## Valid Usage
* If `pos != end()`, `pos` must points to a valid element in the queue. 

