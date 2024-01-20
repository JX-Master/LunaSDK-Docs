# Luna::Simd::transform2d_rotation_f3x4

```c++
float3x4 transform2d_rotation_f3x4(f32 rotation)
```

Builds a 2D affine matrix from roation. 


```
ret[0].x := COS(rotation)
ret[0].y := SIN(rotation)
ret[0].z := 0
ret[0].w := 0
ret[1].x := -SIN(rotation)
ret[1].y := COS(rotation)
ret[1].z := 0
ret[1].w := 0
ret[2].x := 0
ret[2].y := 0
ret[2].z := 1
ret[2].w := 0
```


