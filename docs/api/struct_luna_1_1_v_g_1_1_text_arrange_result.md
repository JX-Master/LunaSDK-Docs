# Luna::VG::TextArrangeResult
Describes text arrange result returned by ITextArranger::arrange. 

```c++
struct Luna::VG::TextArrangeResult
```

## Member objects
* [RectF bounding_rect](struct_luna_1_1_v_g_1_1_text_arrange_result_1a5a8a0b85ace059dd12249c1c922cf4e4.md)

    The real bounding rect occupied by the text. This may be smaller than the bounding rect specified. 

* [bool overflow](struct_luna_1_1_v_g_1_1_text_arrange_result_1a49aa97067a36875627e1380c3fb3833d.md)

    True if the bounding rect is too small to hold all text specified. 

* [Vector<TextLineArrangeResult> lines](struct_luna_1_1_v_g_1_1_text_arrange_result_1a0120e1bb0f2fd1a01e72789870881a8a.md)

    The arrange result of one text lines. 

