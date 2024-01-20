# Luna::Simd::dot4v_f4

```c++
float4 dot4v_f4(float4 a, float4 b)
```

Computes the dot product on elements of `a` and `b`, and stores the result in each element of `dst`. 


```
dp := (a.x * b.x) + (a.y * b.y) + (a.z * b.z) + (a.w * b.w)
dst.x := dp
dst.y := dp
dst.z := dp
dst.w := dp
```


