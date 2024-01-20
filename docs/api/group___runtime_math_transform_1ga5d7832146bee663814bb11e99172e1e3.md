# Luna::AffineMatrix::backward

```c++
Float3 backward(const Float4x4 &affine_matrix)
```

Extracts the backward direction from one 3D affine matrix. 

The returned vector is scaled by the Z factor of the scale component of the affine matrix. 

## Parameters
* *in* **affine_matrix**

    The affine matrix to extract the vector. 

## Return value
Returns the extracted vector. 

