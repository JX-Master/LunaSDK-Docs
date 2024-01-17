# Luna::operator/

```c++
Float3 operator/(const Float3 &v, f32 s)
```

Divides one vector with one scalar. 

This function performs the following operations: 
```
[Float3](struct_luna_1_1_float3.md) r;
r.[x](struct_luna_1_1_float3_1a6b05cac69c0301ab972c27ce208373be.md) = v.x / s;
r.[y](struct_luna_1_1_float3_1ab7291adeb8828a0cba3aedf332c2053d.md) = v.y / s;
r.[z](struct_luna_1_1_float3_1aac280fcf3516d20b5e3dec5fa770ac50.md) = v.z / s;
return r;
```


## Parameters
* *in* **v**

    The vector. 

* *in* **s**

    The scalar. 

## Return value
Returns the result vector. 

