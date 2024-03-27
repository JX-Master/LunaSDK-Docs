# Luna::VG::IShapeDrawList::get_index_buffer

```c++
virtual RHI::IBuffer * get_index_buffer()=0
```

Gets the compiled index buffer used for rendering glyphs in this draw list. 



## Return value
Returns the compiled index buffer. 

## Valid Usage
* This function must be called after calling [compile](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a10a80c3abd16ad8bb629fbb48cd92784.md) in order to let new shape draw commands take effect. 

