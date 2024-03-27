# Luna::VG::IFontAtlas::get_shape_buffer

```c++
virtual R< RHI::IBuffer * > get_shape_buffer()=0
```

Gets the shape buffer that stores the glyph contour commands. 

This call will copy shape command points to the shape buffer using GPU if shape point data is modified after last call to [get_shape_buffer](struct_luna_1_1_v_g_1_1_i_font_atlas_1a0c3982401393c73e890dff86fb9d37e5.md) (or if [get_shape_buffer](struct_luna_1_1_v_g_1_1_i_font_atlas_1a0c3982401393c73e890dff86fb9d37e5.md) is called for the first time after [clear](struct_luna_1_1_v_g_1_1_i_font_atlas_1a5eeb94d22b8366d1b68d0614384802fe.md)), so the user should call this function only if all glyph shapes are packed to the atlas to avoid data copy overhead. 

## Return value
Returns the shape buffer. 

