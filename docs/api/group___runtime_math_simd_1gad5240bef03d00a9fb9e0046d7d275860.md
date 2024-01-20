# Luna::Simd::determinantv_f3x3

```c++
float4 determinantv_f3x3(float3x4 a)
```

Computes the determinant of the 3x3 matrix `a`, and stores the result in every element of `dst`. 


```
DETER :=a[0].x * (a[1].y * a[2].z - a[1].z * a[2].y) +
        a[0].y * (a[1].z * a[2].x - a[1].x * a[2].z) +
        a[0].z * (a[1].x * a[2].y - a[1].y * a[2].x)
dst.x := DETER
dst.y := DETER
dst.z := DETER
dst.w := DETER
```


