# Luna::AffineMatrix::euler_angles

```c++
Float3 euler_angles(const Float4x4 &affine_matrix)
```

Computes the euler angles from one rotation matrix. 

This method cannot be used for affine matrix directly, to use this method for affine matrix, call [rotation_matrix](group___runtime_math_transform_1ga032e2fe95d08cca4b502e7e9f709061a.md) to extract the rotation matrix from affine matrix first.

The returned euler angles represents the radians of clockwise rotation along Z(roll), X(pitch), Y(yaw) axis in that order. 

## Parameters
* *in* **rotation_matrix**

    The rotation matrix. 

## Return value
Returns the rotation represented by euler angles (X = pitch, Y = yaw, Z = roll). 

