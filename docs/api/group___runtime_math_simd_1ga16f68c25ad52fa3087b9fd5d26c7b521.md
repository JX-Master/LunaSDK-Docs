# Luna::Simd::transform3d_rotation_z_f4x4

```c++
float4x4 transform3d_rotation_z_f4x4(f32 rotation)
```

Builds a 3D affine matrix from rotation along Z axis. 


```
S := SIN(rotation)
C := COS(rotation)
ret[0].x := C
ret[0].y := S
ret[0].z := 0
ret[0].w := 0
ret[1].x := -S
ret[1].y := C
ret[1].z := 0
ret[1].w := 0
ret[2].x := 0
ret[2].y := 0
ret[2].z := 1
ret[2].w := 0
ret[3].x := 0
ret[3].y := 0
ret[3].z := 0
ret[3].w := 1
```


