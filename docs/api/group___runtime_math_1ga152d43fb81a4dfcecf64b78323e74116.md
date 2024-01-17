# Luna::determinant

```c++
f32 determinant(const Float4x4 &mat)
```

Computes the determinant of the specified matrix. 

This function performs the following operations: 
```
return
     m.r[0].x * (m.r[1].y * (m.r[2].z * m.r[3].w - m.r[2].w * m.r[3].z) + m.r[1].z * (m.r[2].w * m.r[3].y - m.r[2].y * m.r[3].w) + m.r[1].w * (m.r[2].y * m.r[3].z - m.r[2].z * m.r[3].y))
    -m.r[0].y * (m.r[1].x * (m.r[2].z * m.r[3].w - m.r[2].w * m.r[3].z) + m.r[1].z * (m.r[2].w * m.r[3].x - m.r[2].x * m.r[3].w) + m.r[1].w * (m.r[2].x * m.r[3].z - m.r[2].z * m.r[3].x))
    +m.r[0].z * (m.r[1].x * (m.r[2].y * m.r[3].w - m.r[2].w * m.r[3].y) + m.r[1].y * (m.r[2].w * m.r[3].x - m.r[2].x * m.r[3].w) + m.r[1].w * (m.r[2].x * m.r[3].y - m.r[2].y * m.r[3].x))
    -m.r[0].w * (m.r[1].x * (m.r[2].y * m.r[3].z - m.r[2].z * m.r[3].y) + m.r[1].y * (m.r[2].z * m.r[3].x - m.r[2].x * m.r[3].z) + m.r[1].z * (m.r[2].x * m.r[3].y - m.r[2].y * m.r[3].x));
```


## Parameters
* *in* **mat**

    The matrix to compute. 

## Return value
Returns the computed determinant. 

