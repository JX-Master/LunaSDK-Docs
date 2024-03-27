# Luna::in_bounds

```c++
bool in_bounds(const Float4 &point, const Float4 &min_bound, const Float4 &max_bound)
```

Checks whether the point is in the specified boundary. 

This function performs the following operations: 
```
if (point.x >= min_bound.x && point.x <= max_bound.x 
    && point.y >= min_bound.y && point.y <= max_bound.y
       && point.z >= min_bound.z && point.z <= max_bound.z
       && point.w >= min_bound.w && point.w <= max_bound.w)
    return true;
else return false;
```


## Parameters
* *in* **point**

    The point to check. 

* *in* **min_bound**

    The minimum boundary value. 

* *in* **max_bound**

    The maximum boundary value. 

## Return value
Returns `true` if the point is in the specified boundary. Returns `false` otherwise. 

