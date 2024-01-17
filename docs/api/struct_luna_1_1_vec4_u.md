# Luna::Vec4U
A generalized version of 4D vector. This vector type does not have specific alignment requirement. 

```c++
template <typename _Ty>
struct Luna::Vec4U
```



## Parameters

in] _Ty The element type of the vector. 

## Member objects
* [_Ty x](struct_luna_1_1_vec4_u_1a83d614aa3a837b563ea6c640c5acbd80.md)

    The fist component of the vector. 

* [_Ty y](struct_luna_1_1_vec4_u_1ad50589e0bf2c95d200c5e93a93725ddc.md)

    The second component of the vector. 

* [_Ty z](struct_luna_1_1_vec4_u_1a39f7640e60d9dfd2ae55a31ab2fc86a3.md)

    The third component of the vector. 

* [_Ty w](struct_luna_1_1_vec4_u_1a7600480f5b205176db281c2427dd8de8.md)

    The fourth component of the vector. 

* [_Ty m[4]](struct_luna_1_1_vec4_u_1a287827e5fa68e45eabe383c475d6338a.md)

    The array of components. 

## Member functions
* [Vec4U()=default](struct_luna_1_1_vec4_u_1a1a20ecf09aa85564b445038102aa32f2.md)

    Constructs one vector with components uninitialized. 

* [Vec4U(const Vec4U &)=default](struct_luna_1_1_vec4_u_1ae49d627ae38d209a5b4a49686360ccd3.md)

    Constructs one vector by coping components from another vector. 

* [Vec4U & operator=(const Vec4U &)=default](struct_luna_1_1_vec4_u_1a08d67f9892dda48c1519bf355dcc4660.md)

    Assigns one vector by coping components from another vector. 

* [Vec4U(Vec4U &&)=default](struct_luna_1_1_vec4_u_1a58af14e5569c18be90ec878a382eabf1.md)

    Constructs one vector by coping components from another vector. 

* [Vec4U & operator=(Vec4U &&)=default](struct_luna_1_1_vec4_u_1a738d5f25a35064b3a8d16b7567819b3d.md)

    Assigns one vector by coping components from another vector. 

* [Vec4U(const Float4 &rhs)](struct_luna_1_1_vec4_u_1ad53ba90e64e3d1406c4e7bba6f1c66a9.md)

    Constructs one vector from one [Float4](struct_luna_1_1_float4.md) vector. 

* [Vec4U & operator=(const Float4 &rhs)](struct_luna_1_1_vec4_u_1a40700d3de63727855325b6c51539d31c.md)

    Assigns one vector from one [Float4](struct_luna_1_1_float4.md) vector. 

* [operator Float4() const](struct_luna_1_1_vec4_u_1aa15ef47cb54853f595ac8429a68e8656.md)

    Converts this vector to [Float4](struct_luna_1_1_float4.md). 

* [constexpr Vec4U(_Ty _x)](struct_luna_1_1_vec4_u_1ad20aa30d2dfd46ae440a9eaa9878c192.md)

    Constructs one vector from one scalar. 

* [constexpr Vec4U(_Ty _x, _Ty _y, _Ty _z, _Ty _w)](struct_luna_1_1_vec4_u_1a7c8c4789304696a94500999aa836647b.md)

    Constructs one vector from values. 

* [bool operator==(const Vec4U &rhs) const](struct_luna_1_1_vec4_u_1a1b5bf3ea949213f5693ae752798a4d49.md)

    Compares two vectors for equality. 

* [bool operator!=(const Vec4U &rhs) const](struct_luna_1_1_vec4_u_1aad29fe259dcef3d52a39c86e977aeb8a.md)

    Compares two vectors for non-equality. 

