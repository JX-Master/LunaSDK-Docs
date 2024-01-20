# Luna::ProjectionMatrix::make_orthographic_off_center

```c++
Float4x4 make_orthographic_off_center(f32 left, f32 right, f32 bottom, f32 top, f32 near_z, f32 far_z)
```

Constructs one orthographic projection matrix using four offset values from the camera center, near clipping distance and far clipping distance. 



## Parameters
* *in* **left**

    The offset of the left border of the viewport from camera center. 

* *in* **right**

    The offset of the right border of the viewport from camera center. 

* *in* **bottom**

    The offset of the bottom border of the viewport from camera center. 

* *in* **top**

    The offset of the top border of the viewport from camera center. 

* *in* **near_z**

    The Z position of the near plane. 

* *in* **far_z**

    The Z position of the far plane. 

## Return value
Returns the projection matrix. 

