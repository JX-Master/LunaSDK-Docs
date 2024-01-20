# Luna::Simd::rsqrtest_f4

```c++
float4 rsqrtest_f4(float4 a)
```

Computes the approximate reciprocal square root of packed single-precision (32-bit) floating-point elements in `a`, and stores the results in `dst`. SSE specific: The maximum relative error for this approximation is less than 1.5*2^-12. 


```
dst.x = 1.0 / SQRT(a.x)
dst.y = 1.0 / SQRT(a.y)
dst.z = 1.0 / SQRT(a.z)
dst.w = 1.0 / SQRT(a.w)
```


