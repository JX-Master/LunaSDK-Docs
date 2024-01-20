# Luna::Simd::transform3d_rotation_quaternion_f4x4

```c++
float4x4 transform3d_rotation_quaternion_f4x4(float4 quaternion)
```

Builds a 3D affine matrix from rotation represented by one quaternion. 


```
QX := quaternion.x
QY := quaternion.y
QZ := quaternion.z
QW := quaternion.w
ret[0].x := 1 - 2 * (QY * QY + QZ * QZ)
ret[0].y :=     2 * (QX * QY + QZ * QW)
ret[0].z :=     2 * (QX * QZ - QY * QW)
ret[0].w := 0
ret[1].x :=     2 * (QX * QY - QZ * QW)
ret[1].y := 1 - 2 * (QX * QX + QZ * QZ)
ret[1].z :=     2 * (QY * QZ + QX * QW)
ret[1].w := 0
ret[2].x :=     2 * (QX * QZ + QY * QW)
ret[2].y :=     2 * (QY * QZ - QX * QW)
ret[2].z := 1 - 2 * (QX * QX + QY * QY)
ret[2].w := 0
ret[3].x := 0
ret[3].y := 0
ret[3].z := 0
ret[3].w := 1
```


