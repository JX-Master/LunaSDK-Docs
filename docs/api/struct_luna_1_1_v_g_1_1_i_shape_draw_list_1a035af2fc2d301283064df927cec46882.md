# Luna::VG::IShapeDrawList::draw_shape

```c++
virtual void draw_shape(u32 begin_command, u32 num_commands, const Float2U &min_position, const Float2U &max_position, const Float2U &min_shapecoord, const Float2U &max_shapecoord, u32 color=0xFFFFFFFF, const Float2U &min_texcoord=Float2U(0.0f), const Float2U &max_texcoord=Float2U(0.0f))=0
```

Draws one shape. The shape is drawn by adding one draw rect (two triangles) to the list. 



## Parameters
* *in* **begin_command**

    The index of the first command point of the glyph to draw in shape buffer. 

* *in* **num_commands**

    The number of command points of the glyph to draw. 

* *in* **min_position**

    The minimum position of the bounding rect of the shape. 

* *in* **max_position**

    The maximum position of the bounding rect of the shape. 

* *in* **min_shapecoord**

    The shape coordinate value that maps to the minimum position of the bounding rect of the shape. 

* *in* **max_shapecoord**

    The shape coordinate value that maps to the maximum position of the bounding rect of the shape. 

* *in* **color**

    The color to tint the shape in RGBA8 form. 

* *in* **min_texcoord**

    The texture coordinate value that maps to the minimum position of the bounding rect of the shape. 

* *in* **max_shapecoord**

    The texture coordinate value that maps to the maximum position of the bounding rect of the shape. 

