# Luna::Simd::catmull_rom_f4

```c++
float4 catmull_rom_f4(float4 a, float4 b, float4 c, float4 d, f32 t)
```

Computes Catmull-Rom spline interpolation on packed single-precision (32-bit) floating-point elements in `a`, `b`, `c` and `d` using the single-precision (32-bit) floating-point value `t`, and stores the results in `dst`. 


```
T0 := (-t^3 + 2 * t^2 - t) * 0.5
T1 := (3 * t^3 - 5 * t^2 + 2) * 0.5
T2 := (-3 * t^3 + 4 * t^2 + t) * 0.5
T3 := (t^3 - t^2) * 0.5
FOR j := 0 to 3
    i := j*32
    dst[i:i+31] := T0 * a[i:i+31] + T1 * b[i:i+31] + T2 * c[i:i+31] + T3 * d[i:i+31]
ENDFOR
```


