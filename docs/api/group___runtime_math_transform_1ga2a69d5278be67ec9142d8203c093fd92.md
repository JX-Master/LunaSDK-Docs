# Luna::AffineMatrix::down

```c++
Float2 down(const Float3x3 &affine_matrix)
```

Extracts the down direction from one 2D affine matrix. 

The returned vector is scaled by the Y factor of the scale component of the affine matrix. 

## Parameters
* *in* **affine_matrix**

    The affine matrix to extract the vector. 

## Return value
Returns the extracted vector. 

