# Luna::Font::IFontFile::get_vmetrics

```c++
virtual void get_vmetrics(u32 font_index, i32 *ascent, i32 *descent, i32 *line_gap)=0
```

Gets the metrics information for a font in the vertical side. 

These values are expressed in unscaled coordinates, so you must multiply by the scale factor for a given size. 

## Parameters
* *in* **font_index**

    The index of the font to query. 

* *out* **ascent**

    The coordinate above the baseline the font extends. 

* *out* **descent**

    The coordinate below the baseline the font extends (i.e. it is typically negative). 

* *out* **line_gap**

    The spacing between one row's descent and the next row's ascent, so you should advance the vertical position by "*ascent - *descent + *line_gap" 

