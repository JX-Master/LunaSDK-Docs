# Luna::Simd::normalize2_f4

```c++
float4 normalize2_f4(float4 a)
```

Normalizes the first two elements of `a`, and stores the result in `dst`. 


```
LENGTH := SQRT((a.x * b.x) + (a.y * b.y))
dst.x = a.x / LENGTH
dst.y = a.y / LENGTH
dst.z = a.z / LENGTH
dst.w = a.w / LENGTH
```
 If the length of `a` parameter is 0 or INF, the result is indefinite. 

