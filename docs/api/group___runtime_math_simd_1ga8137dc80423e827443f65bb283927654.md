# Luna::Simd::barycentric_f4

```c++
float4 barycentric_f4(float4 a, float4 b, float4 c, f32 f, f32 g)
```

Computes barycentric interpolation on packed single-precision (32-bit) floating-point elements in `a`, `b` and `c` using the single-precision (32-bit) floating-point values `f` and `g`, and stores the results in `dst`. 


```
FOR j := 0 to 3
    i := j*32
    dst[i:i+31] := a[i:i+31] + (b[i:i+31] - a[i:i+31]) * f + (c[i:i+31] - a[i:i+31]) * g
ENDFOR
```


