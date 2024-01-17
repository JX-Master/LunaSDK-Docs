# Luna::operator*

```c++
Float4 operator*(const Float4 &v, f32 s)
```

Multiplies one vector with one scalar. 

This function performs the following operations: 
```
[Float4](struct_luna_1_1_float4.md) r;
r.[x](struct_luna_1_1_float4_1a6b05cac69c0301ab972c27ce208373be.md) = v.x * s;
r.[y](struct_luna_1_1_float4_1ab7291adeb8828a0cba3aedf332c2053d.md) = v.y * s;
r.[z](struct_luna_1_1_float4_1aac280fcf3516d20b5e3dec5fa770ac50.md) = v.z * s;
r.[w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md) = v.w * s;
return r;
```


## Parameters
* *in* **v**

    The vector. 

* *in* **s**

    The scalar. 

## Return value
Returns the result vector. 

