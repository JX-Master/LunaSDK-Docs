# Luna::Simd::sincos_f4

```c++
float4 sincos_f4(float4 &out_cos, float4 a)
```

Computes the sine and cosine of packed single-precision (32-bit) floating-point elements in `a` expressed in radians, and stores the results in `dst` and `out_cos`. 


```
dst.x := SIN(a.x)
dst.y := SIN(a.y)
dst.z := SIN(a.z)
dst.w := SIN(a.w)
out_cos.x := COS(a.x)
out_cos.y := COS(a.y)
out_cos.z := COS(a.z)
out_cos.w := COS(a.w)
```


