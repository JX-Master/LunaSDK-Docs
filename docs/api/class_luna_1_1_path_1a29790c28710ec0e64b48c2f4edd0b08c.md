# Luna::Path::erase

```c++
iterator erase(const_iterator pos)
```

Removes one name node from the path. 



## Parameters
* *in* **pos**

    The iterator pointing to the name node to be removed. 

## Return value
Returns one iterator pointing to the next name node of the removed name node when iterating nodes. 

## Valid Usage
* `pos` must points to a valid name node in the path. 

