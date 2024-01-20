# Luna::AffineMatrix::make

```c++
Float4x4 make(const Float3 &translation, const Float4 &rotation, const Float3 &scaling)
```

Constructs one 3D affine matrix. 

The transform matrix is composed in scaling-rotation-translation order. 

## Parameters
* *in* **translation**

    The translation vector. 

* *in* **rotation**

    The rotation quaternion. 

* *in* **scaling**

    The scaling vector. 

## Return value
Returns the result matrix. The matrix can be applied to one vector using `mul(vec, mat)`. 

