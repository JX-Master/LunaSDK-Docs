# Luna::Simd::dupw_f4

```c++
float4 dupw_f4(float4 a)
```

Broadcasts the forth element of `a` to every element of `dst`. 


```
dst.x := a.w
dst.y := a.w
dst.z := a.w
dst.w := a.w
```


