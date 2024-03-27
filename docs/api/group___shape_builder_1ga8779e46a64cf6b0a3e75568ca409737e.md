# Luna::VG::ShapeBuilder::add_circle_bordered

```c++
void add_circle_bordered(Vector< f32 > &points, f32 center_x, f32 center_y, f32 radius, f32 border_width, f32 border_offset=0.0f)
```

Adds commands to draw one bordered circle. 



## Parameters
* *in* **points**

    The shape data point buffer to add command to. 

* *in* **center_x**

    The x coordinates of the circle center. 

* *in* **center_y**

    The y coordinates of the circle center. 

* *in* **radius**

    The circle radius. 

* *in* **border_width**

    The width of the border line. 

* *in* **border_offset**

    The offset of the border line relative to the circle border. Positive value makes the border line move outside of the circle, while negative value makes the border line move inside of the circle. 

