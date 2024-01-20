# Luna::Simd::cmpge_f4

```c++
int4 cmpge_f4(float4 a, float4 b)
```

Compares packed single-precision (32-bit) floating-point elements in `a` and `b` for greater-than-or-equal, and stores the results in dst. 


```
dst.x := (a.x >= b.x) ? 0xFFFFFFFF : 0
dst.y := (a.y >= b.y) ? 0xFFFFFFFF : 0
dst.z := (a.z >= b.z) ? 0xFFFFFFFF : 0
dst.w := (a.w >= b.w) ? 0xFFFFFFFF : 0
```


