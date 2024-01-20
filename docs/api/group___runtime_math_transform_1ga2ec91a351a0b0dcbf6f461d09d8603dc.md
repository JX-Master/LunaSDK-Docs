# Luna::ProjectionMatrix::make_orthographic

```c++
Float4x4 make_orthographic(f32 width, f32 height, f32 near_z, f32 far_z)
```

Constructs one orthographic projection matrix using width, height near clipping distance, and far clipping distance. 



## Parameters
* *in* **near_width**

    The width of the viewport. 

* *in* **near_height**

    The height of the viewport. 

* *in* **near_z**

    The Z position of the near plane. 

* *in* **far_z**

    The Z position of the far plane. 

## Return value
Returns the projection matrix. 

