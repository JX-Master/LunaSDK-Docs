# Luna::Simd::scale_f4

```c++
float4 scale_f4(float4 a, f32 b)
```

Scales packed single-precision (32-bit) floating-point elements in `a` using one single-precision (32-bit) floating-point element `b`, and stores the results in `dst`. 


```
dst.x = a.x * b
dst.y = a.y * b
dst.z = a.z * b
dst.w = a.w * b
```


