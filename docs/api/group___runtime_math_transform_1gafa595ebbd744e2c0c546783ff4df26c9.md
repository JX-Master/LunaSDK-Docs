# Luna::ProjectionMatrix::make_perspective_off_center

```c++
Float4x4 make_perspective_off_center(f32 near_left, f32 near_right, f32 near_bottom, f32 near_top, f32 near_z, f32 far_z)
```

Constructs one perspective projection matrix using four offset values from the camera center, near clipping distance and far clipping distance. 



## Parameters
* *in* **near_left**

    The offset of the left border of the near plane from camera center. 

* *in* **near_right**

    The offset of the right border of the near plane from camera center. 

* *in* **near_bottom**

    The offset of the bottom border of the near plane from camera center. 

* *in* **near_top**

    The offset of the top border of the near plane from camera center. 

* *in* **near_z**

    The Z position of the near plane. 

* *in* **far_z**

    The Z position of the far plane. 

## Return value
Returns the projection matrix. 

