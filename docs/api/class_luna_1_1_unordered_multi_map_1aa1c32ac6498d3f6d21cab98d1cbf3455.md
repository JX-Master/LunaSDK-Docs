# Luna::UnorderedMultiMap::reserve

```c++
void reserve(usize new_cap)
```

Expands the bucket buffer so that it can store at least `new_cap` elements without enpanding the bucket buffer again. 



## Parameters
* *in* **new_cap**

    The number of element to reserve. 

## Remark
This function does nothing if `new_cap` is smaller than or equal to [capacity](class_luna_1_1_unordered_multi_map_1ad96bf59cb22e917cbd210ba068e8acb3.md). 

