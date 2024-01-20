# Luna::AffineMatrix::right

```c++
Float2 right(const Float3x3 &affine_matrix)
```

Extracts the right direction from one 2D affine matrix. 

The returned vector is scaled by the X factor of the scale component of the affine matrix. 

## Parameters
* *in* **affine_matrix**

    The affine matrix to extract the vector. 

## Return value
Returns the extracted vector. 

