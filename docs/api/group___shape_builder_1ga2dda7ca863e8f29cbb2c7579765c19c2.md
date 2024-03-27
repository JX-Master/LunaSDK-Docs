# Luna::VG::ShapeBuilder::add_rectangle_bordered

```c++
void add_rectangle_bordered(Vector< f32 > &points, f32 min_x, f32 min_y, f32 max_x, f32 max_y, f32 border_width, f32 border_offset=0.0f)
```

Adds commands to draw one bordered axis-aligned rectangle. 



## Parameters
* *in* **points**

    The shape data point buffer to add command to. 

* *in* **min_x**

    The minimum x coordinates of the rectangle. 

* *in* **min_y**

    The minimum y coordinates of the rectangle. 

* *in* **max_x**

    The maximum x coordinates of the rectangle. 

* *in* **max_y**

    The maximum y coordinates of the rectangle. 

* *in* **border_width**

    The width of the border line. 

* *in* **border_offset**

    The offset of the border line relative to the rectangle border. Positive value makes the border line move outside of the rectangle, while negative value makes the border line move inside of the rectangle. 

