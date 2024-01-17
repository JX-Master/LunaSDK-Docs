# Luna::Quaternion::operator*=

```c++
Quaternion & operator*=(const Quaternion &q)
```

Concatenates two quaternions, and stores the result to this quaternion. 

This function performs the following operations: 
```
this->[x](struct_luna_1_1_quaternion_1a6b05cac69c0301ab972c27ce208373be.md) = q.w * [x](struct_luna_1_1_quaternion_1a6b05cac69c0301ab972c27ce208373be.md) + q.x * [w](struct_luna_1_1_quaternion_1adb390a9d0e1ce3b726f016e547104e35.md) + q.y * [z](struct_luna_1_1_quaternion_1aac280fcf3516d20b5e3dec5fa770ac50.md) - q.z * [y](struct_luna_1_1_quaternion_1ab7291adeb8828a0cba3aedf332c2053d.md);
this->[y](struct_luna_1_1_quaternion_1ab7291adeb8828a0cba3aedf332c2053d.md) = q.w * [y](struct_luna_1_1_quaternion_1ab7291adeb8828a0cba3aedf332c2053d.md) - q.x * [z](struct_luna_1_1_quaternion_1aac280fcf3516d20b5e3dec5fa770ac50.md) + q.y * [w](struct_luna_1_1_quaternion_1adb390a9d0e1ce3b726f016e547104e35.md) + q.z * [x](struct_luna_1_1_quaternion_1a6b05cac69c0301ab972c27ce208373be.md);
this->[z](struct_luna_1_1_quaternion_1aac280fcf3516d20b5e3dec5fa770ac50.md) = q.w * [z](struct_luna_1_1_quaternion_1aac280fcf3516d20b5e3dec5fa770ac50.md) + q.x * [y](struct_luna_1_1_quaternion_1ab7291adeb8828a0cba3aedf332c2053d.md) - q.y * [x](struct_luna_1_1_quaternion_1a6b05cac69c0301ab972c27ce208373be.md) + q.z * [w](struct_luna_1_1_quaternion_1adb390a9d0e1ce3b726f016e547104e35.md);
this->[w](struct_luna_1_1_quaternion_1adb390a9d0e1ce3b726f016e547104e35.md) = q.w * [w](struct_luna_1_1_quaternion_1adb390a9d0e1ce3b726f016e547104e35.md) - q.x * [x](struct_luna_1_1_quaternion_1a6b05cac69c0301ab972c27ce208373be.md) - q.y * [y](struct_luna_1_1_quaternion_1ab7291adeb8828a0cba3aedf332c2053d.md) - q.z * [z](struct_luna_1_1_quaternion_1aac280fcf3516d20b5e3dec5fa770ac50.md);
```


## Parameters
* *in* **q**

    The quaternion to multiply. 

## Return value
Returns `*this`. 

