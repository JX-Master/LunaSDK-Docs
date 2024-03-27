# Luna::Font::load_ttf_font_file

```c++
R< Ref< IFontFile > > load_ttf_font_file(const byte_t *data, usize data_size)
```

Creates a font file object by parsing the provided TTF or TTC font file data. 

To load font file, you should first creates a blob that owns the file data (.ttf or .ttc), then you pass the data to the font system to create a font object for it. The font data will be referenced by font data and should not be changed during the font lifetime. 

## Parameters
* *in* **data**

    The data of the font file. 

* *in* **data_size**

    The data size of the font file. 

## Return value
Returns the created font file object which is initialized using the font data. 

