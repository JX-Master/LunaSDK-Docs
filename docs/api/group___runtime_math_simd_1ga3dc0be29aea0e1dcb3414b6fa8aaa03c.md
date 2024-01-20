# Luna::Simd::reflect4_f4

```c++
float4 reflect4_f4(float4 i, float4 n)
```

Performs reflection operation based on elements of `i` (incident vector) and `n`(normal vector), and stores the refected vector in `dst`. 


```
PROJ := (a.x * b.x) + (a.y * b.y) + (a.z * b.z) + (a.w * b.w)
dst.x = i.x - 2 * PROJ * n.x
dst.y = i.y - 2 * PROJ * n.y
dst.z = i.z - 2 * PROJ * n.z
dst.w = i.w - 2 * PROJ * n.w
```


