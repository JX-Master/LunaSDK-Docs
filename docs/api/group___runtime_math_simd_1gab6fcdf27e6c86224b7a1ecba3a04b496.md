# Luna::Simd::max_f4

```c++
float4 max_f4(float4 a, float4 b)
```

Compare packed single-precision (32-bit) floating-point elements in `a` and `b`, and store packed maximum values in `dst`. SSE specific: `dst` does not follow the IEEE Standard for Floating - Point Arithmetic(IEEE 754) maximum value when inputs are NaN or signed - zero values. 


```
dst.x = MAX(a.x, b.x)
dst.y = MAX(a.y, b.y)
dst.z = MAX(a.z, b.z)
dst.w = MAX(a.w, b.w)
```


