# Luna::VG::IShapeDrawList::draw_shape

```c++
virtual void draw_shape(u32 begin_command, u32 num_commands, const Float2U &min_position, const Float2U &max_position, const Float2U &min_shapecoord, const Float2U &max_shapecoord, u32 color=0xFFFFFFFF, const Float2U &min_texcoord=Float2U(0.0f), const Float2U &max_texcoord=Float2U(0.0f))=0
```

Draws one shape. The shape is drawn by adding one draw rect (two triangles) to the list. 

