# Luna::cross

```c++
Float4 cross(const Float4 &v1, const Float4 &v2, const Float4 &v3)
```

Computes the cross product of two vectors. 

This function performs the following operations: 
```
[Float4](struct_luna_1_1_float4.md) result;
result.[x](struct_luna_1_1_float4_1a6b05cac69c0301ab972c27ce208373be.md) = ((v2.z * v3.w - v2.w * v3.z) * v1.y) - ((v2.y * v3.w - v2.w * v3.y) * v1.z) + ((v2.y * v3.z - v2.z * v3.y) * v1.w);
result.[y](struct_luna_1_1_float4_1ab7291adeb8828a0cba3aedf332c2053d.md) = ((v2.w * v3.z - v2.z * v3.w) * v1.x) - ((v2.w * v3.x - v2.x * v3.w) * v1.z) + ((v2.z * v3.x - v2.x * v3.z) * v1.w);
result.[z](struct_luna_1_1_float4_1aac280fcf3516d20b5e3dec5fa770ac50.md) = ((v2.y * v3.w - v2.w * v3.y) * v1.x) - ((v2.x * v3.w - v2.w * v3.x) * v1.y) + ((v2.x * v3.y - v2.y * v3.x) * v1.w);
result.[w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md) = ((v2.z * v3.y - v2.y * v3.z) * v1.x) - ((v2.z * v3.x - v2.x * v3.z) * v1.y) + ((v2.y * v3.x - v2.x * v3.y) * v1.z);
return result;
```


## Parameters
* *in* **v1**

    The first vector. 

* *in* **v2**

    The second vector. 

## Return value
Returns the cross product of two vectors. 

