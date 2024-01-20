# Luna::Simd::cross3_f4

```c++
float4 cross3_f4(float4 a, float4 b)
```

Computes the cross product on the first three elements of `a` and `b`, and stores the result in each element of `dst`. 


```
dst.x = a.y * b.z - a.z * b.y
dst.y = a.z * b.x - a.x * b.z
dst.z = a.x * b.y - a.y * b.x
dst.w = 0
```


