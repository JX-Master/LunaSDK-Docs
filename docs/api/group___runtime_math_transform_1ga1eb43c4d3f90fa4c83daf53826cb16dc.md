# Luna::AffineMatrix::rotation

```c++
Float4 rotation(const Float4x4 &rotation_matrix)
```

Computes the quaternion from one rotation matrix. 

This method cannot be used for affine matrix directly, to use this method for affine matrix, call [rotation_matrix](group___runtime_math_transform_1ga032e2fe95d08cca4b502e7e9f709061a.md) to extract the rotation matrix from affine matrix first. 

## Parameters
* *in* **rotation_matrix**

    The rotation matrix. 

## Return value
Returns the extracted quaternion. 

