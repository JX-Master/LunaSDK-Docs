# Luna::List::remove

```c++
usize remove(const value_type &value)
```

Removes all elements that are equal to value. 

Elements are compared using `equal_to<_Ty>`. 

## Parameters
* *in* **value**

    The value to test. 

## Return value
Returns the number of elements removed. 

