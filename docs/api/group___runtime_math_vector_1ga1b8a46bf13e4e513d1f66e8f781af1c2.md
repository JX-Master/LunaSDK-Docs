# Luna::operator/

```c++
Float4 operator/(f32 s, const Float4 &v)
```

Divides one scalar with one vector. 

This function performs the following operations: 
```
[Float4](struct_luna_1_1_float4.md) r;
r.[x](struct_luna_1_1_float4_1a6b05cac69c0301ab972c27ce208373be.md) = s / v.x;
r.[y](struct_luna_1_1_float4_1ab7291adeb8828a0cba3aedf332c2053d.md) = s / v.y;
r.[z](struct_luna_1_1_float4_1aac280fcf3516d20b5e3dec5fa770ac50.md) = s / v.z;
r.[w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md) = s / v.w;
return r;
```


## Parameters
* *in* **s**

    The scalar. 

* *in* **v**

    The vector. 

## Return value
Returns the result vector. 

