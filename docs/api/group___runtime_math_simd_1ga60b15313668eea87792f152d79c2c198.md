# Luna::Simd::and_i4

```c++
int4 and_i4(int4 a, int4 b)
```

Computes the bitwise AND of every bit in `a` and `b`, and stores the results in `dst`. 


```
dst.x = AND(a.x, b.x)
dst.y = AND(a.y, b.y)
dst.z = AND(a.z, b.z)
dst.w = AND(a.w, b.w)
```


