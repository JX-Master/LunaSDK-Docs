# Luna::Font::IFontFile::get_glyph_hmetrics

```c++
virtual void get_glyph_hmetrics(u32 font_index, glyph_t glyph, i32 *advance_width, i32 *left_side_bearing)=0
```

Gets the metrics information for a glyph in the horizontal side. 

These values are expressed in unscaled coordinates, so you must multiply by the scale factor for a given size. 

## Parameters
* *in* **font_index**

    The index of the font to query. 

* *in* **glyph**

    The index of the glyph to query. 

* *out* **advance_width**

    The offset from the current horizontal position to the next horizontal position. 

* *out* **left_side_bearing**

    The offset from the current horizontal position to the left edge of the character. 

