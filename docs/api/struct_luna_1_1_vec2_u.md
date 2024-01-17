# Luna::Vec2U
A generalized version of 2D vector. This vector type does not have specific alignment requirement. 

```c++
template <typename _Ty>
struct Luna::Vec2U
```



## Parameters

in] _Ty The element type of the vector. 

## Member objects
* [_Ty x](struct_luna_1_1_vec2_u_1a83d614aa3a837b563ea6c640c5acbd80.md)

    The fist component of the vector. 

* [_Ty y](struct_luna_1_1_vec2_u_1ad50589e0bf2c95d200c5e93a93725ddc.md)

    The second component of the vector. 

* [_Ty m[2]](struct_luna_1_1_vec2_u_1a299b956f4d51ae8b94e03fbf3d9816ce.md)

    The array of components. 

## Member functions
* [Vec2U()=default](struct_luna_1_1_vec2_u_1a8a0a5328beaf1186035397cf899ab657.md)

    Constructs one vector with components uninitialized. 

* [Vec2U(const Vec2U &)=default](struct_luna_1_1_vec2_u_1aaae3706811166171cee7b84cfe47ef83.md)

    Constructs one vector by coping components from another vector. 

* [Vec2U & operator=(const Vec2U &)=default](struct_luna_1_1_vec2_u_1a5b1a93ae050ce0369e6f9b24549926ef.md)

    Assigns one vector by coping components from another vector. 

* [Vec2U(Vec2U &&)=default](struct_luna_1_1_vec2_u_1aeb725059825128685dde784cb306691f.md)

    Constructs one vector by coping components from another vector. 

* [Vec2U & operator=(Vec2U &&)=default](struct_luna_1_1_vec2_u_1ae4164f0e219179d10404750a8e687d97.md)

    Assigns one vector by coping components from another vector. 

* [Vec2U(const Float2 &rhs)](struct_luna_1_1_vec2_u_1a785d8fde946373238d37898ad620a147.md)

    Constructs one vector from one [Float2](struct_luna_1_1_float2.md) vector. 

* [Vec2U & operator=(const Float2 &rhs)](struct_luna_1_1_vec2_u_1a8d0b9b86189e3f5c66d631313381f075.md)

    Assigns one vector from one [Float2](struct_luna_1_1_float2.md) vector. 

* [operator Float2() const](struct_luna_1_1_vec2_u_1a39ce7ff2260db414ecc109a2b5e65f12.md)

    Converts this vector to [Float2](struct_luna_1_1_float2.md). 

* [constexpr Vec2U(_Ty s)](struct_luna_1_1_vec2_u_1a067e2193924163598a861cafce9dbabf.md)

    Constructs one vector from one scalar. 

* [constexpr Vec2U(_Ty x, _Ty y)](struct_luna_1_1_vec2_u_1a1915cd8af9b09a47cff698c60ee49cca.md)

    Constructs one vector from values. 

* [bool operator==(const Vec2U &rhs) const](struct_luna_1_1_vec2_u_1a1500f1e9b47cead3ceca4ae05e3477fb.md)

    Compares two vectors for equality. 

* [bool operator!=(const Vec2U &rhs) const](struct_luna_1_1_vec2_u_1a37f7179c6ccc0cf7ad2f0b78f7b47376.md)

    Compares two vectors for non-equality. 

