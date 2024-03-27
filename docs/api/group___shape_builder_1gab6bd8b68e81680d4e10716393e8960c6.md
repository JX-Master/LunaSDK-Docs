# Luna::VG::ShapeBuilder::circle_to

```c++
void circle_to(Vector< f32 > &points, f32 radius, f32 begin, f32 end)
```

Adds commands to draw one circle part to shape data points. 

If the draw circle part overlaps multiple quadrants, this function seprates the circle part to multiple [COMMAND_CIRCLE_Q1](group___v_g_1gae74f281a578a5f428899d48a20a3de41.md), [COMMAND_CIRCLE_Q2](group___v_g_1gadb09ffc714fbd2dc527b5ec059cf243d.md), [COMMAND_CIRCLE_Q3](group___v_g_1ga0c82be9e0411094ce381166e7f3ad50d.md) and [COMMAND_CIRCLE_Q4](group___v_g_1ga7089bf6633f7ac9d92050e761ba12d4d.md) commands automatically. 

## Parameters
* *in* **points**

    The shape data point buffer to add command to. 

* *in* **radius**

    The radius of the circle. 

* *in* **begin**

    The beginning angle of the circle in degrees. 

* *in* **end**

    The end angle of the circle in degrees. If the end angle is greater than the beginning angle, the circle is drawn counter-clockwisly, otherwise, the circle is drawn clockwisly. 

