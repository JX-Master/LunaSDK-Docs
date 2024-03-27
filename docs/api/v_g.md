# Vector Graphics
[Vector](class_luna_1_1_vector.md) Graphics (VG) module provides functions to render GPU-accelerated vector graphics on 2D or 3D space. 

## Types
* [Luna::VG::IFontAtlas](struct_luna_1_1_v_g_1_1_i_font_atlas.md)

    Represents one font glyph packer that packs font glyph data to one. 


* [Luna::VG::Vertex](struct_luna_1_1_v_g_1_1_vertex.md)

    Describes one vertex to be drawn for the glyph. 


* [Luna::VG::ShapeDrawCall](struct_luna_1_1_v_g_1_1_shape_draw_call.md)

    Describes one shape draw call. 


* [Luna::VG::IShapeDrawList](struct_luna_1_1_v_g_1_1_i_shape_draw_list.md)

    Represents a draw list that contains shapes to be drawn. 


* [Luna::VG::TextGlyphArrangeResult](struct_luna_1_1_v_g_1_1_text_glyph_arrange_result.md)

    Describes the arrange result of one text glyph. 


* [Luna::VG::TextLineArrangeResult](struct_luna_1_1_v_g_1_1_text_line_arrange_result.md)

    Describes the arrange result of one text line that contains multiple glyphs. 


* [Luna::VG::TextArrangeResult](struct_luna_1_1_v_g_1_1_text_arrange_result.md)

    Describes text arrange result returned by ITextArranger::arrange. 


* [Luna::VG::TextArrangeSection](struct_luna_1_1_v_g_1_1_text_arrange_section.md)

    Describes parameters used to arrange one text section. 


## Enumerations
* [Luna::VG::TextAlignment](group___v_g_1gad39fca3b2f0f70c5283dbdb852d65f89.md)

    Specifies the test alignment side. 

## Constants
* [constexpr f32 COMMAND_MOVE_TO](group___v_g_1ga2bc6953cffc02fae8cda53242fae1faf.md)

    The command code that begins one new path. 

* [constexpr f32 COMMAND_LINE_TO](group___v_g_1ga7517475317efab0dc674d8ac0f0ef425.md)

    The command code that draws one line from the last point to the specified point. 

* [constexpr f32 COMMAND_CURVE_TO](group___v_g_1ga24b80fd84c61026f367d5c5d91583621.md)

    The command code that draws a quadratic Belzier curve to the specified point. 

* [constexpr f32 COMMAND_CIRCLE_Q1](group___v_g_1gae74f281a578a5f428899d48a20a3de41.md)

    The command code that draws one circle part in the first quadrant. 

* [constexpr f32 COMMAND_CIRCLE_Q2](group___v_g_1gadb09ffc714fbd2dc527b5ec059cf243d.md)

    The command code that draws one circle part in the second quadrant. 

* [constexpr f32 COMMAND_CIRCLE_Q3](group___v_g_1ga0c82be9e0411094ce381166e7f3ad50d.md)

    The command code that draws one circle part in the third quadrant. 

* [constexpr f32 COMMAND_CIRCLE_Q4](group___v_g_1ga7089bf6633f7ac9d92050e761ba12d4d.md)

    The command code that draws one circle part in the fourth quadrant. 

## Functions
* [Ref< IFontAtlas > new_font_atlas(Font::IFontFile *font, u32 index, RHI::IDevice *device=nullptr)](group___v_g_1gaf3793cd3b220093dd273e2cd0f0fb915.md)

    Creates one new font atlas. 

* [Ref< IShapeDrawList > new_shape_draw_list(RHI::IDevice *device=nullptr)](group___v_g_1ga2519ab312f380880fa9a024d992a7359.md)

    Creates a new shape draw list. 

* [R< Ref< IShapeRenderer > > new_fill_shape_renderer(RHI::ITexture *render_target)](group___v_g_1ga974a394d8c6fa059ae9aa55c7615a8cb.md)

    Creates a new shape renderer that draws filled shape contours. 

* [TextArrangeResult arrange_text(const c8 *text, usize text_len, Span< const TextArrangeSection > sections, const RectF &bounding_rect, TextAlignment vertical_alignment, TextAlignment horizontal_alignment)](group___v_g_1ga352c8c1606f78eb02bd2f3af58b408da.md)

    Arranges glyphs in the specified bounding rectangle. 

* [RV commit_text_arrange_result(const TextArrangeResult &result, Span< const TextArrangeSection > sections, IShapeDrawList *draw_list)](group___v_g_1ga1e2823964d24fe547edbb141f2e384aa.md)

    Commits the text arrange result to the specicied draw list for rendering. 

