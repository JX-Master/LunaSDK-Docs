# Luna::Simd::transform2d_f3x4

```c++
float3x4 transform2d_f3x4(float4 translation, f32 rotation, float4 scaling)
```

Builds a 2D affine matrix from translation, rotation and scaling. 


```
ret[0].x := scaling.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) * COS(rotation)
ret[0].y := scaling.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) * SIN(rotation)
ret[0].z := 0
ret[0].w := 0
ret[1].x := scaling.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) * -SIN(rotation)
ret[1].y := scaling.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) * COS(rotation)
ret[1].z := 0
ret[1].w := 0
ret[2].x := translation.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md)
ret[2].y := translation.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md)
ret[2].z := 1
ret[2].w := 0
```


