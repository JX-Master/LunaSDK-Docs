# Luna::List::merge

```c++
void merge(List &&other)
```

Merges another list into this list. 

No memory allocation or element copy/move will be performed, this function transfers elements by changing their pointers directly so that they link to the new list. Elements are compared using `less<_Ty>`. 

## Parameters
* *in* **other**

    The list to merge. This list will be empty after this operation. If this is equal to `*this`, this function does nothing. 

## Valid Usage
* Elements in `*this` and `other` must be sorted in ascending order. 

