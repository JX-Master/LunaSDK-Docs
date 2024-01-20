# Luna::AffineMatrix::make_look_to

```c++
Float4x4 make_look_to(const Float3 &eye_pos, const Float3 &eye_dir, const Float3 &up_dir)
```

Constructs one view matrix that targets the specified direction. 



## Parameters
* *in* **eye_pos**

    The position of the view point (camera position). 

* *in* **eye_dir**

    The direction to look to. 

* *in* **up_dir**

    The up direction. 

## Return value
Returns the view matrix. 

