# Luna::transpose

```c++
Float3x3 transpose(const Float3x3 &mat)
```

Computes the transpose matrix of the specified matrix. 

This function performs the following operations: 
```
return [Float3x3](struct_luna_1_1_float3x3.md)(
    mat.r[0].x, mat.r[1].x, mat.r[2].x,
    mat.r[0].y, mat.r[1].y, mat.r[2].y,
    mat.r[0].z, mat.r[1].z, mat.r[2].z
);
```


## Parameters
* *in* **mat**

    The matrix to compute. 

## Return value
Returns the transpose matrix of the specified matrix. 

