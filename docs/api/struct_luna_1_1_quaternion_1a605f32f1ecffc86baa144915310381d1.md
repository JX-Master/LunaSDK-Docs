# Luna::Quaternion::operator*=

```c++
Quaternion & operator*=(f32 s)
```

Multiplies this quaternion with one scalar, and stores the result to this quaternion. 

This function performs the following operations: 
```
this->[x](struct_luna_1_1_quaternion_1a6b05cac69c0301ab972c27ce208373be.md) *= s;
this->[y](struct_luna_1_1_quaternion_1ab7291adeb8828a0cba3aedf332c2053d.md) *= s;
this->[z](struct_luna_1_1_quaternion_1aac280fcf3516d20b5e3dec5fa770ac50.md) *= s;
this->[w](struct_luna_1_1_quaternion_1adb390a9d0e1ce3b726f016e547104e35.md) *= s;
```


## Parameters
* *in* **s**

    The scalar to multiply. 

## Return value
Returns `*this`. 

