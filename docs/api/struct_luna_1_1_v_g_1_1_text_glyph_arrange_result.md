# Luna::VG::TextGlyphArrangeResult
Describes the arrange result of one text glyph. 

```c++
struct Luna::VG::TextGlyphArrangeResult
```

## Member objects
* [RectF bounding_rect](struct_luna_1_1_v_g_1_1_text_glyph_arrange_result_1a5a8a0b85ace059dd12249c1c922cf4e4.md)

    The bounding rectangle of the glyph. 

* [f32 origin_offset](struct_luna_1_1_v_g_1_1_text_glyph_arrange_result_1a9daae7dfaf16b166dd613ffcd151d6af.md)

    The orgin point offset of this glyph relative to the beginning of the current line. 

* [f32 advance_length](struct_luna_1_1_v_g_1_1_text_glyph_arrange_result_1ab9b8afb493a00b3506e7d61a48e70e5b.md)

    The advance length of the glyph. This is not always equal to `bounding_rect.width`, because some characters may take more spaces than necessary for paddings. 

* [c32 character](struct_luna_1_1_v_g_1_1_text_glyph_arrange_result_1a449806ea7e774b695b20aadbd9ae5a6a.md)

    The Unicode codepoint of the glyph. 

* [u32 index](struct_luna_1_1_v_g_1_1_text_glyph_arrange_result_1afd715dc311d1a73bd24f87a7624e1bac.md)

    The index of this glyph in the shape buffer of the font atlas. 

