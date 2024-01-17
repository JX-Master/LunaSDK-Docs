# Luna::min

```c++
Float4 min(const Float4 &v1, const Float4 &v2)
```

Computes the minimum value of two vectors. 

This function performs the following operations: 
```
[Float4](struct_luna_1_1_float4.md) result;
result.[x](struct_luna_1_1_float4_1a6b05cac69c0301ab972c27ce208373be.md) = v1.x < v2.x ? v1.x : v2.x;
result.[y](struct_luna_1_1_float4_1ab7291adeb8828a0cba3aedf332c2053d.md) = v1.y < v2.y ? v1.y : v2.y;
result.[z](struct_luna_1_1_float4_1aac280fcf3516d20b5e3dec5fa770ac50.md) = v1.z < v2.z ? v1.z : v2.z;
result.[w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md) = v1.w < v2.w ? v1.w : v2.w;
return result;
```


## Parameters
* *in* **v1**

    The first vector. 

* *in* **v2**

    The second vector. 

## Return value
Returns the minimum value of two vectors. 

