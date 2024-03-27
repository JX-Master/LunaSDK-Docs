# Luna::Simd::hermite_f4

```c++
float4 hermite_f4(float4 v0, float4 t0, float4 v1, float4 t1, f32 t)
```

Computes Hermite spline interpolation on packed single-precision (32-bit) floating-point elements in `v0`, `t0`, `v1` and `t1` using the single-precision (32-bit) floating-point value `t`, and stores the results in `dst`. 


```
P0 := (2 * t^3 - 3 * t^2 + 1)
P1 := (t^3 - 2 * t^2 + t)
P2 := (-2 * t^3 + 3 * t^2)
P3 := (t^3 - t^2)
FOR j := 0 to 3
    i := j*32
       dst[i:i+31] := P0 * v0[i:i+31] + P1 * t0[i:i+31] + P2 * v1[i:i+31] + P3 * t1[i:i+31]
ENDFOR
```


