# Luna::VG::TextLineArrangeResult
Describes the arrange result of one text line that contains multiple glyphs. 

```c++
struct Luna::VG::TextLineArrangeResult
```

## Member objects
* [RectF bounding_rect](struct_luna_1_1_v_g_1_1_text_line_arrange_result_1a5a8a0b85ace059dd12249c1c922cf4e4.md)

    The bounding rect of the line. 

* [f32 baseline_offset](struct_luna_1_1_v_g_1_1_text_line_arrange_result_1a3c15a847a282e52f2bf984471edd792c.md)

    The offset of the baseline of this line. The offset is relative to the starting edge of the text's bounding box. 

* [f32 ascent](struct_luna_1_1_v_g_1_1_text_line_arrange_result_1ac1f1a7807e9667e7d6c98c847227dcc5.md)

    The ascent value (units from baseline to the top of the character) of this line. 

* [f32 decent](struct_luna_1_1_v_g_1_1_text_line_arrange_result_1a3d2df986d526b974c87113c766ebc842.md)

    The decent value (units from baseline to the bottom of the character, typically negative) of this line. 

* [f32 line_gap](struct_luna_1_1_v_g_1_1_text_line_arrange_result_1ac8c89e930fdcdfc20f630f83e73ddfc5.md)

    The line gap of this line. The final line gap is determined by the greater line_gap value of two adjacent lines. 

* [Vector<TextGlyphArrangeResult> glyphs](struct_luna_1_1_v_g_1_1_text_line_arrange_result_1aa8c4fe227f87e6de3a098899a0e7128d.md)

    The arrange result of one text glyphs in this line. 

