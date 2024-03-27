# Luna::VG::ShapeBuilder::curve_to

```c++
void curve_to(Vector< f32 > &points, f32 cx, f32 cy, f32 x, f32 y)
```

Adds one [COMMAND_CURVE_TO](group___v_g_1ga24b80fd84c61026f367d5c5d91583621.md) command to shape data points. 



## Parameters
* *in* **points**

    The shape data point buffer to add command to. 

* *in* **cx**

    The x coordinates of the curve control point. 

* *in* **cy**

    The y coordinates of the curve control point. 

* *in* **x**

    The x coordinates of the target position. 

* *in* **y**

    The y coordinates of the target position. 

