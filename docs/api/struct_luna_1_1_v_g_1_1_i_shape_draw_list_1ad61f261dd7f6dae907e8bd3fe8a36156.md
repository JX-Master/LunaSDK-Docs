# Luna::VG::IShapeDrawList::get_draw_calls

```c++
virtual void get_draw_calls(Vector< ShapeDrawCall > &out_draw_calls)=0
```

Gets an array of draw calls that should be invoked to draw glyphs in this draw list. 



## Parameters
* *out* **out_draw_calls**

    Returns the compiled draw calls. Elements will be pushed to the end of the vector, and existing elements will not be modified. 

