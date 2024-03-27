# Luna::Float4::operator/=

```c++
Float4 & operator/=(const Float4 &v)
```

Divides this vector with one vector, and stores the result to this vector. 

This function performs the following operations: 
```
this->[x](struct_luna_1_1_float4_1a6b05cac69c0301ab972c27ce208373be.md) /= [v](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a9e3669d19b675bd57058fd4664205d2a.md).x;
this->[y](struct_luna_1_1_float4_1ab7291adeb8828a0cba3aedf332c2053d.md) /= [v](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a9e3669d19b675bd57058fd4664205d2a.md).y;
this->[z](struct_luna_1_1_float4_1aac280fcf3516d20b5e3dec5fa770ac50.md) /= [v](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a9e3669d19b675bd57058fd4664205d2a.md).z;
this->[w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md) /= [v](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a9e3669d19b675bd57058fd4664205d2a.md).w;
```


## Parameters
* *in* **v**

    The vector to divide. 

## Return value
Returns `*this`. 

