# Luna::List::List

```c++
List(List &&rhs, const allocator_type &alloc)
```

Constructs a list with an custom allocator and with elements moved from another list. 



## Parameters
### rhs
The list to move elements from. 

### alloc
The allocator to use. The allocator object will be copy-constructed into the list. 

