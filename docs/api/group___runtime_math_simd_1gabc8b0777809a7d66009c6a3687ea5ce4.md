# Luna::Simd::quatnormalangle_f4

```c++
float4 quatnormalangle_f4(float4 n, f32 a)
```

Computes one rotation quaternion based on the given normal `a` and one angle `a`, and stores the result quaternion in `dst`. 


```
SINE := SIN(a * 0.5)
COSINE := COS(a * 0.5)
dst.x := n.x * SINE
dst.y := n.y * SINE
dst.z := n.z * SINE
dst.w := COSINE
```


