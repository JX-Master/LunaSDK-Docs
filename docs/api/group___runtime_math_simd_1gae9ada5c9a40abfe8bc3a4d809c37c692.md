# Luna::Simd::maskint_i4

```c++
i32 maskint_i4(int4 a)
```

Converts the comparison result mask to one 32-bit integer. 


```
FOR j := 0 to 3
    i := j * 32
    IF a[i:i+31] == 0xFFFFFFFF
        dst[j] := 1
    ELSE IF a[i:i+31] == 0x00000000
           dst[j] := 0
       ELSE
           dst[j] := 0 or 1 (The behavior is undefined.)
    FI
ENDFOR
dst[4:MAX] := 0
```


