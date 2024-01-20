# Luna::AffineMatrix::right

```c++
Float3 right(const Float4x4 &affine_matrix)
```

Extracts the right direction. 

The returned vector is scaled by the X factor of the scale component of the affine matrix. 

## Parameters
* *in* **affine_matrix**

    The affine matrix to extract the vector. 

## Return value
Returns the extracted vector. 

