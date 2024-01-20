# Luna::ProjectionMatrix::make_perspective_fov_w

```c++
Float4x4 make_perspective_fov_w(f32 fov_w, f32 aspect_ratio, f32 near_z, f32 far_z)
```

Constructs one perspective projection matrix using width fov, aspect_ratio, near clipping distance and far clipping distance. 



## Parameters
* *in* **fov**

    The width field of view of the camera in radians. 

* *in* **aspect_ratio**

    The aspect ratio (width / height) of the viewport. 

* *in* **near_z**

    The Z position of the near plane. 

* *in* **far_z**

    The Z position of the far plane. 

## Return value
Returns the projection matrix. 

