# Luna::Box
Used to specify a 3D box region using position and size. 

```c++
template <typename _Ty>
struct Luna::Box
```



## Parameters
* **_Ty**

    The type that represents values of the box. 

## Member objects
* [_Ty offset_x](struct_luna_1_1_box_1aad7388b0bd32fe2d41eeacdb94407d02.md)

    The X position of the box. 

* [_Ty offset_y](struct_luna_1_1_box_1a0d685fff6fc97586d48ad4e46782bee3.md)

    The Y position of the box. 

* [_Ty offset_z](struct_luna_1_1_box_1a69f148fb495e37c5ff65698582f0b563.md)

    The Z position of the box. 

* [_Ty height](struct_luna_1_1_box_1a59f3bae4068b3faea664722d71c49350.md)

    The height of the box. 

* [_Ty depth](struct_luna_1_1_box_1a1c14d96a0660834b36710973fd1b66b6.md)

    The depth of the box. 

## Member functions
* [Box()=default](struct_luna_1_1_box_1ab35f0568f1775ad9ae0b7c63c47f0362.md)

    Constructs one box. Values of the box is uninitialized. 

* [Box(_Ty offset_x, _Ty offset_y, _Ty offset_z, _Ty width, _Ty height, _Ty depth)](struct_luna_1_1_box_1ac2f01014f39d92d0db98da79099307b3.md)

    Constructs one box. 

* [bool operator==(const Box &rhs) const](struct_luna_1_1_box_1a06e5f8069dbab70812264246c01f7e62.md)

    Compares two boxes for equality. 

* [bool operator!=(const Box &rhs) const](struct_luna_1_1_box_1aab207b1ddd2f1a9520136b9af42f8e91.md)

    Compares two boxes for non-equality. 

