# Luna::Font::IFontFile::get_kern_advance

```c++
virtual i32 get_kern_advance(u32 font_index, glyph_t ch1, glyph_t ch2)=0
```

Gets an additional amount to add to the 'advance' value between ch1 and ch2. 



## Parameters
* *in* **font_index**

    The index of the font to query. 

* *in* **glyph**

    The index of the first glyph. 

* *in* **glyph**

    The index of the second glyph. 

## Return value
Returns the kern advance between two glyphs in unscaled coordinates. 

