# Luna::Simd::dupz_f4

```c++
float4 dupz_f4(float4 a)
```

Broadcasts the third element of `a` to every element of `dst`. 


```
dst.x := a.z
dst.y := a.z
dst.z := a.z
dst.w := a.z
```


