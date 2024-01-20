# Luna::Simd::quatinverse_f4

```c++
float4 quatinverse_f4(float4 a)
```

Inverts the quaternion `a`, and stores the result in `dst`. 


```
DOT := a.x * a.x + a.y * a.y + a.z * a.z + a.w * a.w;
dst.x := -a.x / DOT;
dst.y := -a.y / DOT;
dst.z := -a.z / DOT;
dst.w :=  a.w / DOT;
```


