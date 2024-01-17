# Luna::OffsetBox
Used to specify a 3D box region using offsets with its container box. 

```c++
template <typename _Ty>
struct Luna::OffsetBox
```



## Parameters
* **_Ty**

    The type that represents values of the box. 

## Member objects
* [_Ty left](struct_luna_1_1_offset_box_1a0027cf811e601b4ef9023ef779830791.md)

    The left offset of the rectangle from its container. 

* [_Ty top](struct_luna_1_1_offset_box_1ad4cc7b2a2468f0afc3bf2714c98d5fd2.md)

    The top offset of the rectangle from its container. 

* [_Ty front](struct_luna_1_1_offset_box_1ab92bec4768e266ea9ec02f39122fe630.md)

    The front offset of the rectangle from its container. 

* [_Ty right](struct_luna_1_1_offset_box_1ac197ccdfbe3c8daabf77f8c3c7f27cab.md)

    The right offset of the rectangle from its container. 

* [_Ty bottom](struct_luna_1_1_offset_box_1a09c6715f60146fa039ef2e2b37aaaca8.md)

    The bottom offset of the rectangle from its container. 

* [_Ty back](struct_luna_1_1_offset_box_1af71bb0bc96aee47925cd3e87fc405a24.md)

    The back offset of the rectangle from its container. 

## Member functions
* [OffsetBox()=default](struct_luna_1_1_offset_box_1a1c2c3be4eb6ea2b4c37b56a4e2d6d42e.md)

    Constructs one box. Values of the box is uninitialized. 

* [OffsetBox(_Ty left, _Ty top, _Ty front, _Ty right, _Ty bottom, _Ty back)](struct_luna_1_1_offset_box_1a41018b40a86106171b16e3b37be9ead7.md)

    Constructs one box. 

* [bool operator==(const OffsetBox &rhs) const](struct_luna_1_1_offset_box_1a675bcb11eae0897a64a31734979608eb.md)

    Compares two boxes for equality. 

* [bool operator!=(const OffsetBox &rhs) const](struct_luna_1_1_offset_box_1a625429c7a7dcaad4c447ab55e4779e1d.md)

    Compares two boxes for non-equality. 

