# Luna::OffsetRect
Used to specify a 2D rectangle region using offsets with its container rectangle. 

```c++
template <typename _Ty>
struct Luna::OffsetRect
```



## Parameters
* **_Ty**

    The type that represents values of the rectangle. 

## Member objects
* [_Ty left](struct_luna_1_1_offset_rect_1a0027cf811e601b4ef9023ef779830791.md)

    The left offset of the rectangle from its container. 

* [_Ty top](struct_luna_1_1_offset_rect_1ad4cc7b2a2468f0afc3bf2714c98d5fd2.md)

    The top offset of the rectangle from its container. 

* [_Ty right](struct_luna_1_1_offset_rect_1ac197ccdfbe3c8daabf77f8c3c7f27cab.md)

    The right offset of the rectangle from its container. 

* [_Ty bottom](struct_luna_1_1_offset_rect_1a09c6715f60146fa039ef2e2b37aaaca8.md)

    The bottom offset of the rectangle from its container. 

## Member functions
* [OffsetRect()=default](struct_luna_1_1_offset_rect_1a8be5bfdcea46ae1a3f7063df983395a0.md)

    Constructs one rectangle. Values of the rectangle is uninitialized. 

* [OffsetRect(_Ty left, _Ty top, _Ty right, _Ty bottom)](struct_luna_1_1_offset_rect_1a67df3d656e8e3023632e08836c0c299d.md)

    Constructs one rectangle. 

* [bool operator==(const OffsetRect &rhs) const](struct_luna_1_1_offset_rect_1ae7b3f618bd30a9aa8f1029a32cdde8f6.md)

    Compares two rectangles for equality. 

* [bool operator!=(const OffsetRect &rhs) const](struct_luna_1_1_offset_rect_1a418a6f44649b2803d5483772d21f1253.md)

    Compares two rectangles for non-equality. 

