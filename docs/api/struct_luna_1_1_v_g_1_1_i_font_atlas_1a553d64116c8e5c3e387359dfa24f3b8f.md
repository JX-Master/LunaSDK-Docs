# Luna::VG::IFontAtlas::get_glyph

```c++
virtual void get_glyph(usize codepoint, usize *first_shape_point, usize *num_shape_points, RectF *bounding_rect)=0
```

Queries the information of the specified glyph, and optionally packs the glyph to this atlas if it is not packed yet. 



## Parameters
* *in* **codepoint**

    The codepoint of the glyph. This is the Unicode of the glyph in most font files. 

* *out* **first_shape_point**

    If not `nullptr`, returns the offset of the first point of the shape in the shape buffer. 

* *out* **num_shape_points**

    If not `nullptr`, returns the number of points of the shape data. 

* *out* **bounding_rect**

    If not `nullptr`, returns the bounding rect of the glyph. 

