# Luna::catmull_rom

```c++
Float3 catmull_rom(const Float3 &v1, const Float3 &v2, const Float3 &vec3, const Float3 &vec4, f32 t)
```

Performs centripetal Catmull–Rom spline interpolation. 

This function performs the following operations: 
```
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) t2 = t * t;
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) t3 = t2 * t;
return (v1 * (-t3 + 2 * t2 - t) +
        v2 * (3 * t3 - 5 * t2 + 2) +
        v3 * (-3 * t3 + 4 * t2 + t) +
        v4 * (t3 - t2)) * 0.5;
```


## Parameters
* *in* **v1**

    The first point of the curve. 

* *in* **v2**

    The second point of the curve. 

* *in* **v3**

    The third point of the curve. 

* *in* **v4**

    The fourth point of the curve. 

* *in* **t**

    The interpolation weight. 

## Return value
Returns the interpolation result. 

