# Luna::Font::IFontFile::get_glyph_shape

```c++
virtual void get_glyph_shape(u32 font_index, glyph_t glyph, Vector< i16 > &out_commands)=0
```

Gets commands in order to draw the specified glyph in unscaled space. 



## Parameters
* *in* **font_index**

    The index of the font to query. 

* *in* **glyph**

    The index of the glyph to query. 

* *out* **out_commands**

    The vector to fetch the returned commands. New commands will be added to the back of the vector, and the existing content in the vector will not be modified. 

