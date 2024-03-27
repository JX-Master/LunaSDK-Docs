# Luna::Font::IFontFile::get_glyph_bounding_box

```c++
virtual RectI get_glyph_bounding_box(u32 font_index, glyph_t glyph)=0
```

Gets the bounding box of the visible part of the glyph. 



## Parameters
* *in* **font_index**

    The index of the font to query. 

* *in* **glyph**

    The index of the glyph to query. 

## Return value
Returns the bounding box of the visible part of the glyph, in unscaled coordinates. 

