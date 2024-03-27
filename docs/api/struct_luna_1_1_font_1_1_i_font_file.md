# Luna::Font::IFontFile
Represents a font file that may contain one or multiple fonts. 

```c++
interface Luna::Font::IFontFile : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual Span< const byte_t > get_data()=0](struct_luna_1_1_font_1_1_i_font_file_1a0c7f071017c95c72510ecbaa1c67ee1e.md)

    Gets the data of the font file. 

* [virtual u32 get_num_fonts()=0](struct_luna_1_1_font_1_1_i_font_file_1a3d158ad591f83663a12352a4200f0206.md)

    Gets the number of fonts in the font file. 

* [virtual glyph_t find_glyph(u32 font_index, u32 codepoint)=0](struct_luna_1_1_font_1_1_i_font_file_1af69d52fc14ced7409e8ddda2d6431896.md)

    Gets the glyph index of the specified character in specified font. 

* [virtual f32 scale_for_pixel_height(u32 font_index, f32 pixels)=0](struct_luna_1_1_font_1_1_i_font_file_1a61184b4868fc41eab8cd29cd1e7d957e.md)

    Computes a scale factor to produce a font whose "height" is `pixels` tall. 

* [virtual void get_vmetrics(u32 font_index, i32 *ascent, i32 *descent, i32 *line_gap)=0](struct_luna_1_1_font_1_1_i_font_file_1acc82f4b6fdff282c883a4c4c39c9ba72.md)

    Gets the metrics information for a font in the vertical side. 

* [virtual void get_glyph_hmetrics(u32 font_index, glyph_t glyph, i32 *advance_width, i32 *left_side_bearing)=0](struct_luna_1_1_font_1_1_i_font_file_1a297aa5cb3c4c5cab20f418191de29f48.md)

    Gets the metrics information for a glyph in the horizontal side. 

* [virtual i32 get_kern_advance(u32 font_index, glyph_t ch1, glyph_t ch2)=0](struct_luna_1_1_font_1_1_i_font_file_1a9fb31d5241c6ad1bae717ed549071c79.md)

    Gets an additional amount to add to the 'advance' value between ch1 and ch2. 

* [virtual void get_glyph_shape(u32 font_index, glyph_t glyph, Vector< i16 > &out_commands)=0](struct_luna_1_1_font_1_1_i_font_file_1a88cdcd806a7dc778e2db6bad217698d3.md)

    Gets commands in order to draw the specified glyph in unscaled space. 

* [virtual RectI get_glyph_bounding_box(u32 font_index, glyph_t glyph)=0](struct_luna_1_1_font_1_1_i_font_file_1a5d826b1e5b846879d5159c8cf0c8ab5d.md)

    Gets the bounding box of the visible part of the glyph. 

* [virtual RectI get_glyph_bitmap_box(u32 font_index, glyph_t glyph, f32 scale_x, f32 scale_y, f32 shift_x, f32 shift_y)=0](struct_luna_1_1_font_1_1_i_font_file_1a41e755b9665ad809a4b2e44d994fc3d0.md)

    Gets the bounding box of the bitmap centered around the glyph origin. 

* [virtual void render_glyph_bitmap(u32 font_index, glyph_t glyph, void *output, i32 out_w, i32 out_h, i32 out_row_pitch, f32 scale_x, f32 scale_y, f32 shift_x, f32 shift_y)=0](struct_luna_1_1_font_1_1_i_font_file_1a24f75306024460827c313121ccb5a138.md)

    Renders a bitmap of the specified glyph into the buffer specified by the `output`., where `out_w` and `out_h` is the width and height. 

