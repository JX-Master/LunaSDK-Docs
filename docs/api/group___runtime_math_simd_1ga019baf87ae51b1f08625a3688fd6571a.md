# Luna::Simd::sin_f4

```c++
float4 sin_f4(float4 a)
```

Computes the sine of packed single-precision (32-bit) floating-point elements in `a` expressed in radians, and stores the results in `dst`. 


```
dst.x := SIN(a.x)
dst.y := SIN(a.y)
dst.z := SIN(a.z)
dst.w := SIN(a.w)
```


