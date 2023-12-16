# Luna::HashSet::reserve

```c++
void reserve(usize new_cap)
```

Expands the data table size to the specified value. 



## Parameters
* *in* **new_cap**

    The new data table size to expand to. 

## Remark
This function does nothing if `new_cap` is smaller than or equal to `capacity()`. 

