# Luna::Simd::transform3d_look_to_f4x4

```c++
float4x4 transform3d_look_to_f4x4(float4 eye, float4 eyedir, float4 updir)
```

Creates one affine matrix that trnasforms points and directions in world space to view space. `eyedir` and `updir` must be normalized. 


```
RZ := eyedir
RX := CROSS3(updir, RZ)
RY := CROSS3(RZ, RX)
TX := DOT3(RX, -eye)
TY := DOT3(RY, -eye)
TZ := DOT3(RZ, -eye)
dst[0] := VEC4(RX.x, RY.x, RZ.x, 0)
dst[1] := VEC4(RX.y, RY.y, RZ.y, 0)
dst[2] := VEC4(RX.z, RY.z, RZ.z, 0)
dst[3] := VEC4(TX, TY, TZ, 1)
```


