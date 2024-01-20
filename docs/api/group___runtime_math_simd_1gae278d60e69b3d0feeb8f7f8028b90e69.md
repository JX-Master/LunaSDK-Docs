# Luna::Simd::matmul_f4x4

```c++
float4x4 matmul_f4x4(float4x4 a, float4x4 b)
```

Performs 4x4 matrix multiplication on `a` and `b`, and stores the result in `dst`. 


```
dst[0].x := a[0].x * b[0].x + a[0].y * b[1].x + a[0].z * b[2].x + a[0].w * b[3].x
dst[0].y := a[0].x * b[0].y + a[0].y * b[1].y + a[0].z * b[2].y + a[0].w * b[3].y
dst[0].z := a[0].x * b[0].z + a[0].y * b[1].z + a[0].z * b[2].z + a[0].w * b[3].z
dst[0].w := a[0].x * b[0].w + a[0].y * b[1].w + a[0].z * b[2].w + a[0].w * b[3].w
dst[1].x := a[1].x * b[0].x + a[1].y * b[1].x + a[1].z * b[2].x + a[1].w * b[3].x
dst[1].y := a[1].x * b[0].y + a[1].y * b[1].y + a[1].z * b[2].y + a[1].w * b[3].y
dst[1].z := a[1].x * b[0].z + a[1].y * b[1].z + a[1].z * b[2].z + a[1].w * b[3].z
dst[1].w := a[1].x * b[0].w + a[1].y * b[1].w + a[1].z * b[2].w + a[1].w * b[3].w
dst[2].x := a[2].x * b[0].x + a[2].y * b[1].x + a[2].z * b[2].x + a[2].w * b[3].x
dst[2].y := a[2].x * b[0].y + a[2].y * b[1].y + a[2].z * b[2].y + a[2].w * b[3].y
dst[2].z := a[2].x * b[0].z + a[2].y * b[1].z + a[2].z * b[2].z + a[2].w * b[3].z
dst[2].w := a[2].x * b[0].w + a[2].y * b[1].w + a[2].z * b[2].w + a[2].w * b[3].w
dst[3].x := a[3].x * b[0].x + a[3].y * b[1].x + a[3].z * b[2].x + a[3].w * b[3].x
dst[3].y := a[3].x * b[0].y + a[3].y * b[1].y + a[3].z * b[2].y + a[3].w * b[3].y
dst[3].z := a[3].x * b[0].z + a[3].y * b[1].z + a[3].z * b[2].z + a[3].w * b[3].z
dst[3].w := a[3].x * b[0].w + a[3].y * b[1].w + a[3].z * b[2].w + a[3].w * b[3].w
```


