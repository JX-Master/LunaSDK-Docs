# Luna::VG::ShapeBuilder::add_line

```c++
void add_line(Vector< f32 > &points, f32 p1_x, f32 p1_y, f32 p2_x, f32 p2_y, f32 width, f32 offset=0.0f)
```

Adds commands to draw one line. 



## Parameters
* *in* **points**

    The shape data point buffer to add command to. 

* *in* **p1_x**

    The x coordinates of the first point. 

* *in* **p1_y**

    The y coordinates of the first point. 

* *in* **p2_x**

    The x coordinates of the second point. 

* *in* **p2_y**

    The y coordinates of the second point. 

* *in* **width**

    The line width. 

* *in* **offset**

    The offset of the drawn line relative to the original line formed by two points, in the perpendicular direction of the line direction. 

