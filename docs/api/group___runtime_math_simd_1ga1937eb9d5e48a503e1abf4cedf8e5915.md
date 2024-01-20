# Luna::Simd::dupy_f4

```c++
float4 dupy_f4(float4 a)
```

Broadcasts the second element of `a` to every element of `dst`. 


```
dst.x := a.y
dst.y := a.y
dst.z := a.y
dst.w := a.y
```


