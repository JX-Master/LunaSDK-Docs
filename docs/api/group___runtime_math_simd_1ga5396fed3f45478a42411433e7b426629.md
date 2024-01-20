# Luna::Simd::dot2v_f4

```c++
float4 dot2v_f4(float4 a, float4 b)
```

Computes the dot product on the first two elements of `a` and `b`, and stores the result in each element of `dst`. 


```
dp := (a.x * b.x) + (a.y * b.y)
dst.x := dp
dst.y := dp
dst.z := dp
dst.w := dp
```


