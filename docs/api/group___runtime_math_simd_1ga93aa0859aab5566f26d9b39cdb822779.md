# Luna::Simd::rsqrt_f4

```c++
float4 rsqrt_f4(float4 a)
```

Computes the reciprocal square root of packed single-precision (32-bit) floating-point elements in `a`, and stores the results in `dst`. 


```
dst.x = 1.0 / SQRT(a.x)
dst.y = 1.0 / SQRT(a.y)
dst.z = 1.0 / SQRT(a.z)
dst.w = 1.0 / SQRT(a.w)
```


