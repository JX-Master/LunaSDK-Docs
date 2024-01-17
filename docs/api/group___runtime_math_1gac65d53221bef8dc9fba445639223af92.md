# Luna::determinant

```c++
f32 determinant(const Float3x3 &mat)
```

Computes the determinant of the specified matrix. 

This function performs the following operations: 
```
return
    mat.r[0].x * (mat.r[1].y * mat.r[2].z - mat.r[1].z * mat.r[2].y) +
    mat.r[0].y * (mat.r[1].z * mat.r[2].x - mat.r[1].x * mat.r[2].z) +
    mat.r[0].z * (mat.r[1].x * mat.r[2].y - mat.r[1].y * mat.r[2].x);
```


## Parameters
* *in* **mat**

    The matrix to compute. 

## Return value
Returns the computed determinant. 

