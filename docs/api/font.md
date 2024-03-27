# Font
Font module provides functions to parse font file, extract glyph shape and render glyph bitmap using CPU. 

## Types
* [Luna::Font::IFontFile](struct_luna_1_1_font_1_1_i_font_file.md)

    Represents a font file that may contain one or multiple fonts. 


## Alias types
* [using glyph_t =  i32](group___font_1gaaef0d8989955f1af6ec8c01c6935119e.md)

    The index type of one font glyph. 

## Constants
* [constexpr glyph_t INVALID_GLYPH](group___font_1gaefe7566e5e06c31173b27f643095fd16.md)

    A special index value that identifies one invalid glyph. 

* [constexpr i16 COMMAND_MOVE_TO](group___font_1ga578e438da544148987c569a15b09ee1f.md)

    The command value that starts a new contour, followed by two data points: x, y. 

* [constexpr i16 COMMAND_LINE_TO](group___font_1ga3a3843f46bd2b939e5982acf8abcf460.md)

    The command value that draws a line to the specified point, followed by two data points: x, y. 

* [constexpr i16 COMMAND_CURVE_TO](group___font_1ga67e58caf5bb6b060d6db4d604a7b0a80.md)

    The command value that draws a Quadratic Belzier curve to the specified point, followed by four data points: cx, cy, x, y. 

## Functions
* [R< Ref< IFontFile > > load_ttf_font_file(const byte_t *data, usize data_size)](group___font_1ga54f5e6c1af6417e13dd8c93d862cdd1d.md)

    Creates a font file object by parsing the provided TTF or TTC font file data. 

* [IFontFile * get_default_font()](group___font_1gabfd2db9fe3bf4b1331c2fa7c7cc01c17.md)

    Gets the default font object, which is embedded into the SDK and only supports for ASCII codepoint range. 

