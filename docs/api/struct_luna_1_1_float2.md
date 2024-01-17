# Luna::Float2
2D vector type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 

```c++
struct Luna::Float2
```

This vector type is 16-bytes aligned and will use SIMD to accelerate vector calculations when possible. 

## Member objects
* [f32 x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md)

    The fist component of the vector. 

* [f32 y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md)

    The second component of the vector. 

* [f32 m[2]](struct_luna_1_1_float2_1a00e1f347f78a7c24788f1c21b23f8e14.md)

    The array of components. 

## Member functions
* [Float2()=default](struct_luna_1_1_float2_1a0c053e42a3750cf70f417bfe07c215fa.md)

    Constructs one vector with components uninitialized. 

* [Float2(const Float2 &)=default](struct_luna_1_1_float2_1a9d5a99f668f93f9ee3c4a6b5c75288e5.md)

    Constructs one vector by coping components from another vector. 

* [Float2 & operator=(const Float2 &)=default](struct_luna_1_1_float2_1a29fa375c8753b660e1ea94b9cf008adc.md)

    Assigns one vector by coping components from another vector. 

* [Float2(Float2 &&)=default](struct_luna_1_1_float2_1ab624f1de3bd0746ff3bf41fe42b4e7c5.md)

    Constructs one vector by coping components from another vector. 

* [Float2 & operator=(Float2 &&)=default](struct_luna_1_1_float2_1a48c9b1589274634d5f3a490e55580e42.md)

    Assigns one vector by coping components from another vector. 

* [constexpr Float2(f32 s)](struct_luna_1_1_float2_1aa28bfa90a16de0437fe605da9d4ace24.md)

    Constructs one vector from one scalar. 

* [constexpr Float2(f32 x, f32 y)](struct_luna_1_1_float2_1ab9d4f3fd56e27d4e5d4cc40cca69c9c0.md)

    Constructs one vector from values. 

* [bool operator==(const Float2 &v) const](struct_luna_1_1_float2_1aff5e39ce0efe5dbc41d2fdf9ba814521.md)

    Compares two vectors for equality. 

* [bool operator!=(const Float2 &v) const](struct_luna_1_1_float2_1ab662a2122abc8096229e96c4151ec19b.md)

    Compares two vectors for non-equality. 

* [Float2 & operator+=(const Float2 &v)](struct_luna_1_1_float2_1a6fc3cfb8d47f85a04df693e3702c5659.md)

    Adds this vector with one vector, and stores the result to this vector. 

* [Float2 & operator-=(const Float2 &v)](struct_luna_1_1_float2_1a7a998d28df06a4d367a635c8026b7e15.md)

    Subtracts this vector with one vector, and stores the result to this vector. 

* [Float2 & operator*=(const Float2 &v)](struct_luna_1_1_float2_1adb4e0e53f550a8282408eada6d7fbca2.md)

    Multiplies this vector with one vector, and stores the result to this vector. 

* [Float2 & operator/=(const Float2 &v)](struct_luna_1_1_float2_1afa83f92fdbb3c5495a7a65ffe95a3e36.md)

    Divides this vector with one vector, and stores the result to this vector. 

* [Float2 & operator+=(f32 s)](struct_luna_1_1_float2_1ad8613657abd62edd369ec89fe92e2215.md)

    Adds this vector with one scalar, and stores the result to this vector. 

* [Float2 & operator-=(f32 s)](struct_luna_1_1_float2_1acf6fd1ed0b8fc7d0b422dcf8b22b1198.md)

    Subtracts this vector with one scalar, and stores the result to this vector. 

* [Float2 & operator*=(f32 s)](struct_luna_1_1_float2_1aaf13bc75e0fd2f8180b84e21d35ed0e6.md)

    Multiplies this vector with one scalar, and stores the result to this vector. 

* [Float2 & operator/=(f32 s)](struct_luna_1_1_float2_1a815a34c15ffa50401abd1a19615fe78b.md)

    Divides this vector with one scalar, and stores the result to this vector. 

* [Float2 operator+() const](struct_luna_1_1_float2_1ad1550d574281a43bc7a88dc4c8e1a19e.md)

    Gets the vector as-is. 

* [Float2 operator-() const](struct_luna_1_1_float2_1a953596bab0aa83a5c4310f8043245fe0.md)

    Gets a negation of this vector. 

