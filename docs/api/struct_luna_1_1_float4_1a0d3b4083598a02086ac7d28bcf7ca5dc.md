# Luna::Float4::operator*=

```c++
Float4 & operator*=(const Float4 &v)
```

Multiplies this vector with one vector, and stores the result to this vector. 

This function performs the following operations: 
```
this->[x](struct_luna_1_1_float4_1a6b05cac69c0301ab972c27ce208373be.md) *= v.x;
this->[y](struct_luna_1_1_float4_1ab7291adeb8828a0cba3aedf332c2053d.md) *= v.y;
this->[z](struct_luna_1_1_float4_1aac280fcf3516d20b5e3dec5fa770ac50.md) *= v.z;
this->[w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md) *= v.w;
```


## Parameters
* *in* **v**

    The vector to multiply. 

## Return value
Returns `*this`. 

