# Luna::VG::IShapeDrawList::draw_shape_raw

```c++
virtual void draw_shape_raw(Span< const Vertex > vertices, Span< const u32 > indices)=0
```

Draws one shape by submitting vertices and indices directly. 



## Parameters
* *in* **vertices**

    The draw vertices. 

* *in* **indices**

    The draw indices. Valid index range is [`0`, `vertices.size()`). 

