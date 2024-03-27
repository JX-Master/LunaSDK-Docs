# Luna::Simd::inverse_f3x3

```c++
float3x4 inverse_f3x3(float3x4 a, f32 *out_determinant)
```

Computes the determinant and the inverse matrix of `a`, stores the determinant in `out_determinant`, and stores the inverse matrix in `dst`. 


```
   DETER :=a[0].x * (a[1].y * a[2].z - a[1].z * a[2].y) +
           a[0].y * (a[1].z * a[2].x - a[1].x * a[2].z) +
           a[0].z * (a[1].x * a[2].y - a[1].y * a[2].x)
IF out_determinant != 0
       MEM[out_determinant:out_determinant+31] := DETER
ENDIF
INV_DETER := 1.0 / DETER
dst[0].x := INV_DETER * (a[1].y * a[2].z - a[1].z * a[2].y);
dst[1].x := INV_DETER * (a[1].z * a[2].x - a[1].x * a[2].z);
dst[2].x := INV_DETER * (a[1].x * a[2].y - a[1].y * a[2].x);
dst[0].y := INV_DETER * (a[0].z * a[2].y - a[0].y * a[2].z);
dst[1].y := INV_DETER * (a[0].x * a[2].z - a[0].z * a[2].x);
dst[2].y := INV_DETER * (a[0].y * a[2].x - a[0].x * a[2].y);
dst[0].z := INV_DETER * (a[0].y * a[1].z - a[0].z * a[1].y);
dst[1].z := INV_DETER * (a[0].z * a[1].x - a[0].x * a[1].z);
dst[2].z := INV_DETER * (a[0].x * a[1].y - a[0].y * a[1].x);
```
 The forth element of every row of `a` is indefinite. If `DETER` is 0, `dst` is indefinite. 

