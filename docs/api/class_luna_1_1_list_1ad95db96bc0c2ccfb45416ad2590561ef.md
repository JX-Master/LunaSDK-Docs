# Luna::List::unique

```c++
usize unique()
```

Removes all consecutive duplicate elements from the container. 

Only the first element in each group of equal elements is left. Elements are compared using `[equal_to](struct_luna_1_1equal__to.md)<_Ty>`. 

## Return value
Returns the number of elements removed. 

