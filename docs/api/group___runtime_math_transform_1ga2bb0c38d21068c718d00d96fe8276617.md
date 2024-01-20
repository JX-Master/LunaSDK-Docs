# Luna::AffineMatrix::make

```c++
Float3x3 make(const Float2 &translation, f32 rotation, const Float2 &scaling)
```

Constructs one 2D affine matrix. 

The transform matrix is composed in scaling-rotation-translation order. 

## Parameters
* *in* **translation**

    The translation vector. 

* *in* **rotation**

    The rotation represented in radians. 

* *in* **scaling**

    The scaling vector. 

## Return value
Returns the result matrix. The matrix can be applied to one vector using `mul(vec, mat)`. 

