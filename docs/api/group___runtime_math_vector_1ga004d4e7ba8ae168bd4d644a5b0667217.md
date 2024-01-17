# Luna::hermite

```c++
Float4 hermite(const Float4 &v1, const Float4 &t1, const Float4 &v2, const Float4 &t2, f32 t)
```

Performs Hermite spline interpolation. 

This function performs the following operations: 
```
[Float4](struct_luna_1_1_float4.md) result;
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) t2 = t * t;
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) t3 = t2 * t;
return  v1 * (2 * t3 - 3 * t2 + 1) +
        t1 * (t3 - 2 * t2 + t) +
        v3 * (-2 * t3 + 3 * t2) +
        t2 * (t3 - t2);
```


## Parameters
* *in* **v1**

    The first point of the curve. 

* *in* **t1**

    The first tangent of the curve. 

* *in* **v2**

    The second point of the curve. 

* *in* **t2**

    The second tangent of the curve. 

* *in* **t**

    The interpolation weight. 

## Return value
Returns the interpolation result. 

