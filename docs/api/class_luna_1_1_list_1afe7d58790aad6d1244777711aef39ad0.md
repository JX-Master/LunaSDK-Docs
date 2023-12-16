# Luna::List::resize

```c++
void resize(usize count)
```

Changes the number of elements in the list. 



## Parameters
* *in* **count**

    The new size of the list. If this is larger than `size()`, new elements will be default-inserted at the back of the list. If this is smaller than `size()`, elements in range [`count`, `size()`) will be removed from the list. If this is equal to `size()`, this function does nothing. 

