# Luna::Simd::quateulerangles_f4

```c++
float4 quateulerangles_f4(float4 a)
```

Computes a rotation quaternion based on a vector containing the Euler angles (pitch, yaw, and roll), and stores the result in `dst`. 


```
PITCH := a.x
YAW   := a.y
ROLL  := a.z
SP  := SIN(PITCH * 0.5)
CP  := COS(PITCH * 0.5)
SY  := SIN(YAW * 0.5)
CY  := COS(YAW * 0.5)
SR  := SIN(ROLL * 0.5)
CR  := COS(ROLL * 0.5)
dst.x := CR * SP * CY + SR * CP * SY
dst.y := CR * CP * SY - SR * SP * CY
dst.z := SR * CP * CY - CR * SP * SY
dst.w := CR * CP * CY + SR * SP * SY
```


