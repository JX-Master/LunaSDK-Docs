# Luna::Simd::mulquat_f4

```c++
float4 mulquat_f4(float4 a, float4 b)
```

Multiplies two quaternion `a` and `b`, and stores the result in `dst`. 


```
dst.x := (a.x * b.w) + (a.w * b.x) + (a.z * b.y) - (a.y * b.z)
dst.y := (a.y * b.w) - (a.z * b.x) + (a.w * b.y) + (a.x * b.z)
dst.z := (a.z * b.w) + (a.y * b.x) - (a.x * b.y) + (a.w * b.z)
dst.w := (a.w * b.w) - (a.x * b.x) - (a.y * b.y) - (a.z * b.z)
```


