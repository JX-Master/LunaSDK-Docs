# Luna::Simd::determinantv_f4x4

```c++
float4 determinantv_f4x4(float4x4 a)
```

Calculates the determinant of matrix `a`, and stores the result in every element of `dst`. 


```
DETER := a[0].x * (a[1].y * (a[2].z * a[3].w - a[2].w * a[3].z) + a[1].z * (a[2].w * a[3].y - a[2].y * a[3].w) + a[1].w * (a[2].y * a[3].z - a[2].z * a[3].y))
        -a[0].y * (a[1].x * (a[2].z * a[3].w - a[2].w * a[3].z) + a[1].z * (a[2].w * a[3].x - a[2].x * a[3].w) + a[1].w * (a[2].x * a[3].z - a[2].z * a[3].x))
        +a[0].z * (a[1].x * (a[2].y * a[3].w - a[2].w * a[3].y) + a[1].y * (a[2].w * a[3].x - a[2].x * a[3].w) + a[1].w * (a[2].x * a[3].y - a[2].y * a[3].x))
        -a[0].w * (a[1].x * (a[2].y * a[3].z - a[2].z * a[3].y) + a[1].y * (a[2].z * a[3].x - a[2].x * a[3].z) + a[1].z * (a[2].x * a[3].y - a[2].y * a[3].x))
dst.x := DETER
dst.y := DETER
dst.z := DETER
dst.w := DETER
```


