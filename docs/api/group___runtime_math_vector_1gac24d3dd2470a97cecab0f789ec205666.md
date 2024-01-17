# Luna::distance_squared

```c++
f32 distance_squared(const Float2 &v1, const Float2 &v2)
```

Computes the squared distance between two points. 

This function performs the following operations: 
```
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) dx = v1.x - v2.x;
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) dy = v1.y - v2.y;
return dx * dx + dy * dy;
```


## Parameters
* *in* **v1**

    The first point. 

* *in* **v2**

    The second point. 

## Return value
Returns the squared distance between two points. 

