# Luna::List::unique

```c++
usize unique()
```

Removes all consecutive duplicate elements from the container. 

Only the first element in each group of equal elements is left. Elements are compared using `equal_to<_Ty>`. 

## Return value
Returns the number of elements removed. 

