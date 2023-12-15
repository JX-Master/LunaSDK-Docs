# Luna::List::splice

```c++
void splice(const_iterator pos, List &&other, const_iterator it)
```

Transfers one element from another list to this list. 

## Overview
No memory allocation or element copy/move will be performed, this function transfers elements by changing their pointers directly so that they link to the new list. 

## Parameters
### pos
The iterator pointing to the position to insert the transferred element. 

### other
The list to transfer the element from. 

### it
The iterator pointing to the element to be transferred. 

