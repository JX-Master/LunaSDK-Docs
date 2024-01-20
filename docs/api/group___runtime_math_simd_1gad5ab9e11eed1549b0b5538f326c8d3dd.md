# Luna::Simd::negmuladd_f4

```c++
float4 negmuladd_f4(float4 a, float4 b, float4 c)
```

Multiply packed single-precision (32-bit) floating-point elements in `a` and `b`, add the negated intermediate result to packed elements in `c`, and store the results in dst. 


```
dst.x = -(a.x * b.x) + c.x
dst.y = -(a.y * b.y) + c.y
dst.z = -(a.z * b.z) + c.z
dst.w = -(a.w * b.w) + c.w
```


