# Luna::Simd::scaleadd_f4

```c++
float4 scaleadd_f4(float4 a, f32 b, float4 c)
```

Scales packed single-precision (32-bit) floating-point elements in `a` using one single-precision (32-bit) floating-point element `b`, add the intermediate result to packed elements in `c`, and stores the results in `dst`. 


```
dst.x = (a.x * b) + c.x
dst.y = (a.y * b) + c.y
dst.z = (a.z * b) + c.z
dst.w = (a.w * b) + c.w
```


