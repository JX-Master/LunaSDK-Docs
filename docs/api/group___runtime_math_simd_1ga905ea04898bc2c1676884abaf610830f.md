# Luna::Simd::matmul_f3x3

```c++
float3x4 matmul_f3x3(float3x4 a, float3x4 b)
```

Performs 3x3 matrix multiplication on `a` and `b`, and stores the result in `dst`. 


```
dst[0].x := a[0].x * b[0].x + a[0].y * b[1].x + a[0].z * b[2].x
dst[0].y := a[0].x * b[0].y + a[0].y * b[1].y + a[0].z * b[2].y
dst[0].z := a[0].x * b[0].z + a[0].y * b[1].z + a[0].z * b[2].z
dst[1].x := a[1].x * b[0].x + a[1].y * b[1].x + a[1].z * b[2].x
dst[1].y := a[1].x * b[0].y + a[1].y * b[1].y + a[1].z * b[2].y
dst[1].z := a[1].x * b[0].z + a[1].y * b[1].z + a[1].z * b[2].z
dst[2].x := a[2].x * b[0].x + a[2].y * b[1].x + a[2].z * b[2].x
dst[2].y := a[2].x * b[0].y + a[2].y * b[1].y + a[2].z * b[2].y
dst[2].z := a[2].x * b[0].z + a[2].y * b[1].z + a[2].z * b[2].z
```
 The forth element of every row of `dst` is indefinite. 

