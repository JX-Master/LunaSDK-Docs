# Luna::RingDeque::erase

```c++
iterator erase(const_iterator first, const_iterator last)
```

Removes one range of elements from the queue. 



## Parameters
* *in* **first**

    The iterator to the first element to be removed. 

* *in* **last**

    The iterator to the one-past-last element to be removed. 

## Return value
Returns one iterator to the next element after the removed elements, or `end()` if such element does not exist. 

## Valid Usage
* `first` must be either `end()` or one valid element in the queue.

* If `first != end()`, [`first`, `last`) must specifies either one empty range (`first == last`) or one valid element range of the queue.

* If `first == end()`, [`first`, `last`) must specifies one empty range (`first == last`). 

