# Luna::Font::IFontFile::find_glyph

```c++
virtual glyph_t find_glyph(u32 font_index, u32 codepoint)=0
```

Gets the glyph index of the specified character in specified font. 



## Parameters
* *in* **font_index**

    The index of the font to query. 

* *in* **codepoint**

    The codepoint of the glyph. 

## Return value
Returns the glyph index of the specified character. 

