# Luna::VG::arrange_text

```c++
TextArrangeResult arrange_text(const c8 *text, usize text_len, Span< const TextArrangeSection > sections, const RectF &bounding_rect, TextAlignment vertical_alignment, TextAlignment horizontal_alignment)
```

Arranges glyphs in the specified bounding rectangle. 



## Parameters
* *in* **text**

    The UTF-8 text to arrange. 

* *in* **text_len**

    The length of `text. If this is @ref USIZE_MAX, the text length is determined by`strlen(text)`. 

* *in* **sections**

    The text arrange sections. Every section may use a different set of text arrange parameters. 

* *in* **bounding_rect**

    The bounding rectangle to arrange text in. 

* *in* **vertical_alignment**

    The vertical alignment for text lines. 

* *in* **horizontal_alignment**

    The horizontal alignment for text lines. 

## Return value
Returns the text arrange result. 

