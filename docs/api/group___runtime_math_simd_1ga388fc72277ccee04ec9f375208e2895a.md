# Luna::Simd::transpose_f4x4

```c++
float4x4 transpose_f4x4(float4x4 a)
```

Performs matrix transpose on `a`, and stores the result in `dst`. 


```
dst[0].x = a[0].x
dst[0].y = a[1].x
dst[0].z = a[2].x
dst[0].w = a[3].x
dst[1].x = a[0].y
dst[1].y = a[1].y
dst[1].z = a[2].y
dst[1].w = a[3].y
dst[2].x = a[0].z
dst[2].y = a[1].z
dst[2].z = a[2].z
dst[2].w = a[3].z
dst[3].x = a[0].w
dst[3].y = a[1].w
dst[3].z = a[2].w
dst[3].w = a[3].w
```


