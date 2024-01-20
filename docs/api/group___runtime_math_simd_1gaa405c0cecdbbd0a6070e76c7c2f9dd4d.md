# Luna::Simd::cos_f4

```c++
float4 cos_f4(float4 a)
```

Computes the cosine of packed single-precision (32-bit) floating-point elements in `a` expressed in radians, and stores the results in `dst`. 


```
dst.x := COS(a.x)
dst.y := COS(a.y)
dst.z := COS(a.z)
dst.w := COS(a.w)
```


