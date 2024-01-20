# Luna::Simd::transform3d_rotation_y_f4x4

```c++
float4x4 transform3d_rotation_y_f4x4(f32 rotation)
```

Builds a 3D affine matrix from rotation along Y axis. 


```
S := SIN(rotation)
C := COS(rotation)
ret[0].x := C
ret[0].y := 0
ret[0].z := -S
ret[0].w := 0
ret[1].x := 0
ret[1].y := 1
ret[1].z := 0
ret[1].w := 0
ret[2].x := S
ret[2].y := 0
ret[2].z := C
ret[2].w := 0
ret[3].x := 0
ret[3].y := 0
ret[3].z := 0
ret[3].w := 1
```


