# Luna::operator*

```c++
Float4 operator*(f32 s, const Float4 &v)
```

Multiplies one vector with one scalar. 

This function performs the following operations: 
```
[Float4](struct_luna_1_1_float4.md) r;
r.x = v.x * s;
r.y = v.y * s;
r.z = v.z * s;
r.w = v.w * s;
return r;
```


## Parameters
* *in* **s**

    The scalar. 

* *in* **v**

    The vector. 

## Return value
Returns the result vector. 

