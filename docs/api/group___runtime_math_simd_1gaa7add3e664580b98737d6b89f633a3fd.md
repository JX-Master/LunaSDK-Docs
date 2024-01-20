# Luna::Simd::transform3d_translation_f4x4

```c++
float4x4 transform3d_translation_f4x4(float4 translation)
```

Builds a 3D affine matrix from translation. 


```
ret[0].x := 1
ret[0].y := 0
ret[0].z := 0
ret[0].w := 0
ret[1].x := 0
ret[1].y := 1
ret[1].z := 0
ret[1].w := 0
ret[2].x := 0
ret[2].y := 0
ret[2].z := 1
ret[2].w := 0
ret[3].x := translation.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md)
ret[3].y := translation.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md)
ret[3].z := translation.z
ret[3].w := 1
```


