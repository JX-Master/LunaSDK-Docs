# Luna::ProjectionMatrix::make_perspective

```c++
Float4x4 make_perspective(f32 near_width, f32 near_height, f32 near_z, f32 far_z)
```

Constructs one perspective projection matrix using width, height, near clipping distance and far clipping distance. 



## Parameters
* *in* **near_width**

    The width of the near plane. 

* *in* **near_height**

    The height of the near plane. 

* *in* **near_z**

    The Z position of the near plane. 

* *in* **far_z**

    The Z position of the far plane. 

## Return value
Returns the projection matrix. 

