# Luna::Simd::setzero_f4x4

```c++
float4x4 setzero_f4x4()
```

Returns matrix of type `float4x4` with all elements set to zero. 


```
FOR r := 0 to 3
       dst[r].x := 0
       dst[r].y := 0
       dst[r].z := 0
       dst[r].w := 0
ENDFOR
```


