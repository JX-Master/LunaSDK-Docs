# Luna::Font::IFontFile::get_glyph_bitmap_box

```c++
virtual RectI get_glyph_bitmap_box(u32 font_index, glyph_t glyph, f32 scale_x, f32 scale_y, f32 shift_x, f32 shift_y)=0
```

Gets the bounding box of the bitmap centered around the glyph origin. 



## Parameters
* *in* **font_index**

    The index of the font to query. 

* *in* **glyph**

    The index of the glyph to query. 

* *in* **scale_x**

    The scale factor in horizontal direction. 

* *in* **scale_y**

    The scale factor in vertical direction. 

* *in* **shift_x**

    The value to shift bitmap bounding box in horizontal direction in pixels. 

* *in* **shift_y**

    The value to shift bitmap bounding box in vertical direction in pixels. 

## Remark
The location to place the bitmap top left is (`left_side_bearing * scale_x + shift_x`, `shift_y`). Note that the bitmap uses y-increases-down, but the shape uses y-increases-up, so [get_glyph_bitmap_box](struct_luna_1_1_font_1_1_i_font_file_1a41e755b9665ad809a4b2e44d994fc3d0.md) and [get_glyph_bounding_box](struct_luna_1_1_font_1_1_i_font_file_1a5d826b1e5b846879d5159c8cf0c8ab5d.md) are inverted. 

