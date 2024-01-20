# Luna::Simd::refract4_f4

```c++
float4 refract4_f4(float4 i, float4 n, f32 index)
```

Performs refraction operation based on elements of `i` (incident vector), `n`(normal vector) and the scalar value `index` (refraction index), and stores the refected vector in `dst`. 


```
PROJ := (a.x * b.x) + (a.y * b.y) + (a.z * b.z) + (a.w * b.w)
DETER := 1.0 - index * index  * (1.0 - PROJ * PROJ)
FOR j := 0 to 4
    i := j*32
    IF DETER >= 0
        dst[i:i+31] := index * i[i:i+31] - n[i:i+31] * (index * PROJ + SQRT(DETER))
    ELSE
        dst[i:i+31] := 0
    ENDIF
ENDFOR
```
`i` and `n` should be properly normalized before calling this function.

`index` is `Ni/Nt`, where `Ni` is the refraction index of incident media, and `Nt` is the refraction index of the transmission media. 

