# Luna::List::splice

```c++
void splice(const_iterator pos, List &other, const_iterator first, const_iterator last)
```

Transfers elements from another list to this list. 

No memory allocation or element copy/move will be performed, this function transfers elements by changing their pointers directly so that they link to the new list. 

## Parameters
* *in* **pos**

    The iterator pointing to the position to insert the transferred elements. 

* *in* **other**

    The list to transfer elements from. 

* *in* **first**

    The iterator pointing to the first element to be transferred. 

* *in* **last**

    The iterator pointing to the one-past-last element to be transferred. 

