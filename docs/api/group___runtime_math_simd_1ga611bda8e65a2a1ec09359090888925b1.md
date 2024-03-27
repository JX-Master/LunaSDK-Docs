# Luna::Simd::inverse_f4x4

```c++
float4x4 inverse_f4x4(float4x4 a, f32 *out_determinant)
```

Computes the determinant and the inverse matrix of `a`, stores the determinant in `out_determinant`, and stores the inverse matrix in `dst`. 


```
DETER := a[0].x * (a[1].y * (a[2].z * a[3].w - a[2].w * a[3].z) + a[1].z * (a[2].w * a[3].y - a[2].y * a[3].w) + a[1].w * (a[2].y * a[3].z - a[2].z * a[3].y))
           -a[0].y * (a[1].x * (a[2].z * a[3].w - a[2].w * a[3].z) + a[1].z * (a[2].w * a[3].x - a[2].x * a[3].w) + a[1].w * (a[2].x * a[3].z - a[2].z * a[3].x))
           +a[0].z * (a[1].x * (a[2].y * a[3].w - a[2].w * a[3].y) + a[1].y * (a[2].w * a[3].x - a[2].x * a[3].w) + a[1].w * (a[2].x * a[3].y - a[2].y * a[3].x))
           -a[0].w * (a[1].x * (a[2].y * a[3].z - a[2].z * a[3].y) + a[1].y * (a[2].z * a[3].x - a[2].x * a[3].z) + a[1].z * (a[2].x * a[3].y - a[2].y * a[3].x))
IF out_determinant != 0
       MEM[out_determinant:out_determinant+31] := DETER
ENDIF
INV_DETER := 1.0 / DETER
dst[0].x :=  INV_DETER * (a[1].y * (a[2].z * a[3].w - a[2].w * a[3].z) + a[1].z * (a[2].w * a[3].y - a[2].y * a[3].w) + a[1].w * (a[2].y * a[3].z - a[2].z * a[3].y));
dst[1].x := -INV_DETER * (a[1].x * (a[2].z * a[3].w - a[2].w * a[3].z) + a[1].z * (a[2].w * a[3].x - a[2].x * a[3].w) + a[1].w * (a[2].x * a[3].z - a[2].z * a[3].x));
dst[2].x :=  INV_DETER * (a[1].x * (a[2].y * a[3].w - a[2].w * a[3].y) + a[1].y * (a[2].w * a[3].x - a[2].x * a[3].w) + a[1].w * (a[2].x * a[3].y - a[2].y * a[3].x));
dst[3].x := -INV_DETER * (a[1].x * (a[2].y * a[3].z - a[2].z * a[3].y) + a[1].y * (a[2].z * a[3].x - a[2].x * a[3].z) + a[1].z * (a[2].x * a[3].y - a[2].y * a[3].x));
dst[0].y := -INV_DETER * (a[0].y * (a[2].z * a[3].w - a[2].w * a[3].z) + a[0].z * (a[2].w * a[3].y - a[2].y * a[3].w) + a[0].w * (a[2].y * a[3].z - a[2].z * a[3].y));
dst[1].y :=  INV_DETER * (a[0].x * (a[2].z * a[3].w - a[2].w * a[3].z) + a[0].z * (a[2].w * a[3].x - a[2].x * a[3].w) + a[0].w * (a[2].x * a[3].z - a[2].z * a[3].x));
dst[2].y := -INV_DETER * (a[0].x * (a[2].y * a[3].w - a[2].w * a[3].y) + a[0].y * (a[2].w * a[3].x - a[2].x * a[3].w) + a[0].w * (a[2].x * a[3].y - a[2].y * a[3].x));
dst[3].y :=  INV_DETER * (a[0].x * (a[2].y * a[3].z - a[2].z * a[3].y) + a[0].y * (a[2].z * a[3].x - a[2].x * a[3].z) + a[0].z * (a[2].x * a[3].y - a[2].y * a[3].x));
dst[0].z :=  INV_DETER * (a[3].w * (a[0].y * a[1].z - a[0].z * a[1].y) + a[3].z * (a[0].w * a[1].y - a[0].y * a[1].w) + a[3].y * (a[0].z * a[1].w - a[0].w * a[1].z));
dst[1].z := -INV_DETER * (a[3].w * (a[0].x * a[1].z - a[0].z * a[1].x) + a[3].z * (a[0].w * a[1].x - a[0].x * a[1].w) + a[3].x * (a[0].z * a[1].w - a[0].w * a[1].z));
dst[2].z :=  INV_DETER * (a[3].w * (a[0].x * a[1].y - a[0].y * a[1].x) + a[3].y * (a[0].w * a[1].x - a[0].x * a[1].w) + a[3].x * (a[0].y * a[1].w - a[0].w * a[1].y));
dst[3].z := -INV_DETER * (a[3].z * (a[0].x * a[1].y - a[0].y * a[1].x) + a[3].y * (a[0].z * a[1].x - a[0].x * a[1].z) + a[3].x * (a[0].y * a[1].z - a[0].z * a[1].y));
dst[0].w := -INV_DETER * (a[2].w * (a[0].y * a[1].z - a[0].z * a[1].y) + a[2].z * (a[0].w * a[1].y - a[0].y * a[1].w) + a[2].y * (a[0].z * a[1].w - a[0].w * a[1].z));
dst[1].w :=  INV_DETER * (a[2].w * (a[0].x * a[1].z - a[0].z * a[1].x) + a[2].z * (a[0].w * a[1].x - a[0].x * a[1].w) + a[2].x * (a[0].z * a[1].w - a[0].w * a[1].z));
dst[2].w := -INV_DETER * (a[2].w * (a[0].x * a[1].y - a[0].y * a[1].x) + a[2].y * (a[0].w * a[1].x - a[0].x * a[1].w) + a[2].x * (a[0].y * a[1].w - a[0].w * a[1].y));
dst[3].w :=  INV_DETER * (a[2].z * (a[0].x * a[1].y - a[0].y * a[1].x) + a[2].y * (a[0].z * a[1].x - a[0].x * a[1].z) + a[2].x * (a[0].y * a[1].z - a[0].z * a[1].y));
```
 If `DETER` is 0, `dst` is indefinite. 

