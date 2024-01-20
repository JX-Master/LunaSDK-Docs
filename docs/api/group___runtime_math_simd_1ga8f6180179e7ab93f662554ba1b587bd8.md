# Luna::Simd::cross2_f4

```c++
float4 cross2_f4(float4 a, float4 b)
```

Computes the cross product on the first two elements of `a` and `b`, and stores the result in `dst`. 


```
cp := (a.x * b.y) - (a.y * b.x)
dst.x := cp
dst.y := cp
dst.z := cp
dst.w := cp
```


