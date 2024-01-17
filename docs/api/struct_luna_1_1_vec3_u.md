# Luna::Vec3U
A generalized version of 3D vector. This vector type does not have specific alignment requirement. 

```c++
template <typename _Ty>
struct Luna::Vec3U
```



## Parameters

in] _Ty The element type of the vector. 

## Member objects
* [_Ty x](struct_luna_1_1_vec3_u_1a83d614aa3a837b563ea6c640c5acbd80.md)

    The fist component of the vector. 

* [_Ty y](struct_luna_1_1_vec3_u_1ad50589e0bf2c95d200c5e93a93725ddc.md)

    The second component of the vector. 

* [_Ty z](struct_luna_1_1_vec3_u_1a39f7640e60d9dfd2ae55a31ab2fc86a3.md)

    The third component of the vector. 

* [_Ty m[3]](struct_luna_1_1_vec3_u_1a269fb9d2792d1ea27c8d7dbfa5052f38.md)

    The array of components. 

## Member functions
* [Vec3U()=default](struct_luna_1_1_vec3_u_1a141cd63cc6e06fec6c0e5c5a6664ec18.md)

    Constructs one vector with components uninitialized. 

* [Vec3U(const Vec3U &)=default](struct_luna_1_1_vec3_u_1aaebadde563d185d64450d11bb710b305.md)

    Constructs one vector by coping components from another vector. 

* [Vec3U & operator=(const Vec3U &)=default](struct_luna_1_1_vec3_u_1aa3ae548a882635ee4b0b7eb751ad4221.md)

    Assigns one vector by coping components from another vector. 

* [Vec3U(Vec3U &&)=default](struct_luna_1_1_vec3_u_1a29a86b44a544708ce61b2a5e8415cb43.md)

    Constructs one vector by coping components from another vector. 

* [Vec3U & operator=(Vec3U &&)=default](struct_luna_1_1_vec3_u_1a8db84643893115e30a6b65e9d67e95c6.md)

    Assigns one vector by coping components from another vector. 

* [Vec3U(const Float3 &rhs)](struct_luna_1_1_vec3_u_1a38a037b796f344d5809c1e5a8469c999.md)

    Constructs one vector from one [Float3](struct_luna_1_1_float3.md) vector. 

* [Vec3U & operator=(const Float3 &rhs)](struct_luna_1_1_vec3_u_1a39181b6988ddd21a910481a5d1ce07ff.md)

    Assigns one vector from one [Float3](struct_luna_1_1_float3.md) vector. 

* [operator Float3() const](struct_luna_1_1_vec3_u_1ae8bdb89842794c0c122f02034717d22e.md)

    Converts this vector to [Float3](struct_luna_1_1_float3.md). 

* [constexpr Vec3U(_Ty s)](struct_luna_1_1_vec3_u_1a30da76c7e69b2721088727e581dfc565.md)

    Constructs one vector from one scalar. 

* [constexpr Vec3U(_Ty x, _Ty y, _Ty z)](struct_luna_1_1_vec3_u_1a540b912e911ccf43855ae9176920b3a0.md)

    Constructs one vector from values. 

* [bool operator==(const Vec3U &rhs) const](struct_luna_1_1_vec3_u_1ae098b0dd714b366e9fdee2fec9028480.md)

    Compares two vectors for equality. 

* [bool operator!=(const Vec3U &rhs) const](struct_luna_1_1_vec3_u_1a739b8d28a626a1340be3a0b5ccab4cca.md)

    Compares two vectors for non-equality. 

