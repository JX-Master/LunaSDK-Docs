# Luna::transpose

```c++
Float4x4 transpose(const Float4x4 &mat)
```

Computes the transpose matrix of the specified matrix. 

This function performs the following operations: 
```
return [Float4x4](struct_luna_1_1_float4x4.md)(
    mat.r[0].x, mat.r[1].x, mat.r[2].x, mat.r[3].x,
    mat.r[0].y, mat.r[1].y, mat.r[2].y, mat.r[3].y,
    mat.r[0].z, mat.r[1].z, mat.r[2].z, mat.r[3].z,
    mat.r[0].w, mat.r[1].w, mat.r[2].w, mat.r[3].w
);
```


## Parameters
* *in* **mat**

    The matrix to compute. 

## Return value
Returns the transpose matrix of the specified matrix. 

