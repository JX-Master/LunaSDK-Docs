# Luna::Simd::cross4_f4

```c++
float4 cross4_f4(float4 a, float4 b, float4 c)
```

Computes the cross product on elements of `a`, `b` and `c`, and stores the result in each element of `dst`. 


```
dst.x = ((b.z * c.w - b.w * c.z) * a.y) - ((b.y * c.w - b.w * c.y) * a.z) + ((b.y * c.z - b.z * c.y) * a.w)
dst.y = ((b.w * c.z - b.z * c.w) * a.x) - ((b.w * c.x - b.x * c.w) * a.z) + ((b.z * c.x - b.x * c.z) * a.w)
dst.z = ((b.y * c.w - b.w * c.y) * a.x) - ((b.x * c.w - b.w * c.x) * a.y) + ((b.x * c.y - b.y * c.x) * a.w)
dst.w = ((b.z * c.y - b.y * c.z) * a.x) - ((b.z * c.x - b.x * c.z) * a.y) + ((b.y * c.x - b.x * c.y) * a.z)
```


