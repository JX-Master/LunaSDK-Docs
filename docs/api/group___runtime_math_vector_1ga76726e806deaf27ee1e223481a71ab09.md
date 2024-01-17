# Luna::distance_squared

```c++
f32 distance_squared(const Float3 &v1, const Float3 &v2)
```

Computes the squared distance between two points. 

This function performs the following operations: 
```
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) dx = v1.x - v2.x;
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) dy = v1.y - v2.y;
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) dz = v1.z - v2.z;
return dx * dx + dy * dy + dz * dz;
```


## Parameters
* *in* **v1**

    The first point. 

* *in* **v2**

    The second point. 

## Return value
Returns the squared distance between two points. 

