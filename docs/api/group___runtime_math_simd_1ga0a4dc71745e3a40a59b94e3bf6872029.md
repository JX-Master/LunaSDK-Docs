# Luna::Simd::lerp_f4

```c++
float4 lerp_f4(float4 a, float4 b, f32 t)
```

Computes linear interpolation on packed single-precision (32-bit) floating-point elements in `a` and `b` using the single-precision (32-bit) floating-point value `t`, and stores the results in `dst`. 

``` FOR j := 0 to 3 i := j*32 dst[i:i+31] := a[i:i+31] + t * (b[i:i+31] - a[i:i+31]) ENDFOR 

