# Luna::Simd::min_f4

```c++
float4 min_f4(float4 a, float4 b)
```

Compare packed single-precision (32-bit) floating-point elements in `a` and `b`, and store packed minimum values in `dst`. SSE specific: `dst` does not follow the IEEE Standard for Floating - Point Arithmetic(IEEE 754) minimum value when inputs are NaN or signed - zero values. 


```
dst.x = MIN(a.x, b.x)
dst.y = MIN(a.y, b.y)
dst.z = MIN(a.z, b.z)
dst.w = MIN(a.w, b.w)
```


