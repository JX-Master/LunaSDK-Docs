# Luna::AffineMatrix::make_look_at

```c++
Float4x4 make_look_at(const Float3 &eye_pos, const Float3 &target_pos, const Float3 &up_dir)
```

Constructs one view matrix that targets the specified position. 



## Parameters
* *in* **eye_pos**

    The position of the view point (camera position). 

* *in* **target_pos**

    The position of the point to look at. 

* *in* **up_dir**

    The up direction. 

## Return value
Returns the view matrix. 

