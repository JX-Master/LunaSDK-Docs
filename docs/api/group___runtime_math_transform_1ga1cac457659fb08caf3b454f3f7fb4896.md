# Luna::AffineMatrix::left

```c++
Float2 left(const Float3x3 &affine_matrix)
```

Extracts the left direction from one 2D affine matrix. 

The returned vector is scaled by the X factor of the scale component of the affine matrix. 

## Parameters
* *in* **affine_matrix**

    The affine matrix to extract the vector. 

## Return value
Returns the extracted vector. 

