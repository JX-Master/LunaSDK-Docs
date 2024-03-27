# Luna::VG::IShapeDrawList::get_index_buffer_size

```c++
virtual u32 get_index_buffer_size()=0
```

Gets the number of indices in the index buffer returned by [get_index_buffer](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a333c05d6272805cec5f22b3a66ab8679.md). 



## Return value
Returns the number of indices in the index buffer. 

## Valid Usage
* This function must be called after calling [compile](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a10a80c3abd16ad8bb629fbb48cd92784.md) in order to let new shape draw commands take effect. 

