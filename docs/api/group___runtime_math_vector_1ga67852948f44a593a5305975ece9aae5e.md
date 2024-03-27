# Luna::operator*

```c++
Float3 operator*(const Float3 &v, f32 s)
```

Multiplies one vector with one scalar. 

This function performs the following operations: 
```
[Float3](struct_luna_1_1_float3.md) r;
r.x = v.x * s;
r.y = v.y * s;
r.z = v.z * s;
return r;
```


## Parameters
* *in* **v**

    The vector. 

* *in* **s**

    The scalar. 

## Return value
Returns the result vector. 

