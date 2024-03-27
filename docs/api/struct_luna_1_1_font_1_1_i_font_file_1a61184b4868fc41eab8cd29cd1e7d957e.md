# Luna::Font::IFontFile::scale_for_pixel_height

```c++
virtual f32 scale_for_pixel_height(u32 font_index, f32 pixels)=0
```

Computes a scale factor to produce a font whose "height" is `pixels` tall. 

Height is measured as the distance from the highest ascender to the lowest descender; in other words, it's equivalent to calling [get_vmetrics](struct_luna_1_1_font_1_1_i_font_file_1acc82f4b6fdff282c883a4c4c39c9ba72.md) and computing: scale = pixels / (ascent - descent) so if you prefer to measure height by the ascent only, use a similar calculation. 

## Parameters
* *in* **font_index**

    The index of the font to query. 

* *in* **pixels**

    The new hight of the font glyphs. 

## Return value
Returns the scale factor. 

