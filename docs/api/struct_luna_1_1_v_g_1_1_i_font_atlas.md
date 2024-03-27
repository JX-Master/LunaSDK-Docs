# Luna::VG::IFontAtlas
Represents one font glyph packer that packs font glyph data to one. 

```c++
interface Luna::VG::IFontAtlas : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual void clear()=0](struct_luna_1_1_v_g_1_1_i_font_atlas_1a5eeb94d22b8366d1b68d0614384802fe.md)

    Removes all glyphs in the font atlas, but keeps the internal storage, so that they can be reused to store new glyphs. 

* [virtual Font::IFontFile * get_font(u32 *index)=0](struct_luna_1_1_v_g_1_1_i_font_atlas_1a05d716c49a685cce7bb78e46fca915f3.md)

    Gets the font file data bound to this font atlas. 

* [virtual void set_font(Font::IFontFile *font, u32 index)=0](struct_luna_1_1_v_g_1_1_i_font_atlas_1af657ff48ae04b535dee1fb4dd093d586.md)

    Sets the font bound to this font atlas. The will reset the font atlas. 

* [virtual R< RHI::IBuffer * > get_shape_buffer()=0](struct_luna_1_1_v_g_1_1_i_font_atlas_1a0c3982401393c73e890dff86fb9d37e5.md)

    Gets the shape buffer that stores the glyph contour commands. 

* [virtual Span< const f32 > get_shape_points()=0](struct_luna_1_1_v_g_1_1_i_font_atlas_1a334e5fe90f439c62266a0fda32b784e7.md)

    Gets the shape points data. 

* [virtual void get_glyph(usize codepoint, usize *first_shape_point, usize *num_shape_points, RectF *bounding_rect)=0](struct_luna_1_1_v_g_1_1_i_font_atlas_1a553d64116c8e5c3e387359dfa24f3b8f.md)

    Queries the information of the specified glyph, and optionally packs the glyph to this atlas if it is not packed yet. 

