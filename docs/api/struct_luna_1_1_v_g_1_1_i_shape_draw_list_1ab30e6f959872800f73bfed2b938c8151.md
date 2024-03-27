# Luna::VG::IShapeDrawList::get_vertex_buffer_size

```c++
virtual u32 get_vertex_buffer_size()=0
```

Gets the number of vertices in the vertex buffer returned by [get_vertex_buffer](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1ab23811de65131965317b15e443f11b1d.md). 



## Return value
Returns the number of vertices in the vertex buffer. 

## Valid Usage
* This function must be called after calling [compile](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a10a80c3abd16ad8bb629fbb48cd92784.md) in order to let new shape draw commands take effect. 

