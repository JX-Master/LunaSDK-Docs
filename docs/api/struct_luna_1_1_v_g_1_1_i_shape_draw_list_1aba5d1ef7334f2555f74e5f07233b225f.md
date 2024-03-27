# Luna::VG::IShapeDrawList::set_shape_buffer

```c++
virtual void set_shape_buffer(RHI::IBuffer *shape_buffer)=0
```

Sets the shape buffer used for the following draw calls. 



## Parameters
* *in* **shape_buffer**

    The shape buffer to set. If this is `nullptr`, the internal shape buffer will be set. 

## Remark
The shape buffer is similar to "glyph atlas texture" in VG. However, instead of storing bitmaps of glyphs like traditional atlas texture, the shape buffer stores command points that describe contours of glyphs. Command points are stored as an array of 32-bit floating-point values and can be read by GPU shader to generate high-resolution graphics by performing scanline testing against contours directly.


One shape buffer may contain contours of multiple glyphs, each glyph takes one continuous range of command points in the shape buffer. The shape buffer can be pre-generated and bind to one shape draw list directly by calling [set_shape_buffer](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1aba5d1ef7334f2555f74e5f07233b225f.md). This is useful if the user wish to draw static glyphs like font characters, since such glyphs never change during run-time, the user can pack all needed glyphs to one shape buffer, and use that shape buffer to draw glyphs directly. If the user does not want to create shape buffer herself, she can also pass `nullptr` to [set_shape_buffer](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1aba5d1ef7334f2555f74e5f07233b225f.md) to use the shape draw list's internal shape buffer. The internal shape buffer is designed to draw contours that may change every frame, like the GUI widget that are generated at runtime, and the data of the internal shape buffer will be cleared every time [reset](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a20dcbdfbd0ec77afc802522bb7e379c1.md) is called. 

