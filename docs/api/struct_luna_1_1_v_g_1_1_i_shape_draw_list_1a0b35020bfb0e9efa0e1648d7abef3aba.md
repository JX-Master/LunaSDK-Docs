# Luna::VG::IShapeDrawList::set_origin

```c++
virtual void set_origin(const Float2 &origin)=0
```

Sets the origin point for the following draw calls. The origin point is relative to the origin point of the canvas. The origin point of the canvas is at the bottom-left corner. The x axis points to right and the y axis points to up. 

The origin point is (0,0) when the draw list has been reset. 

## Parameters
* *in* **offset**

    The x and y offset in pixels. 

