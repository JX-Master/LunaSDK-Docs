# Luna::operator/

```c++
Float2 operator/(const Float2 &v, f32 s)
```

Divides one vector with one scalar. 

This function performs the following operations: 
```
[Float2](struct_luna_1_1_float2.md) r;
r.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) = v.x / s;
r.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) = v.y / s;
return r;
```


## Parameters
* *in* **v**

    The vector. 

* *in* **s**

    The scalar. 

## Return value
Returns the result vector. 

