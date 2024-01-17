# Luna::Float4
4D vector type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 

```c++
struct Luna::Float4
```

This vector type is 16-bytes aligned and will use SIMD to accelerate vector calculations when possible. 

## Member objects
* [f32 x](struct_luna_1_1_float4_1a6b05cac69c0301ab972c27ce208373be.md)

    The fist component of the vector. 

* [f32 y](struct_luna_1_1_float4_1ab7291adeb8828a0cba3aedf332c2053d.md)

    The second component of the vector. 

* [f32 z](struct_luna_1_1_float4_1aac280fcf3516d20b5e3dec5fa770ac50.md)

    The third component of the vector. 

* [f32 w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md)

    The fourth component of the vector. 

* [f32 m[4]](struct_luna_1_1_float4_1a913c09d0cc2a1dab1ceb500fd8704174.md)

    The array of components. 

## Member functions
* [Float4()=default](struct_luna_1_1_float4_1aaafd49eb1f30971d0eeb427e953e94d9.md)

    Constructs one vector with components uninitialized. 

* [Float4(const Float4 &)=default](struct_luna_1_1_float4_1a670c70d6fd9b39fd6313048684674328.md)

    Constructs one vector by coping components from another vector. 

* [Float4 & operator=(const Float4 &)=default](struct_luna_1_1_float4_1ab37539e37291e5ed5bc509d195caab50.md)

    Assigns one vector by coping components from another vector. 

* [Float4(Float4 &&)=default](struct_luna_1_1_float4_1a74c860b926600956ddfa13b5a7adda4b.md)

    Constructs one vector by coping components from another vector. 

* [Float4 & operator=(Float4 &&)=default](struct_luna_1_1_float4_1ab81d6375a4023743728df153e4611660.md)

    Assigns one vector by coping components from another vector. 

* [constexpr Float4(f32 s)](struct_luna_1_1_float4_1a347eaab3d24379521c3d7090ac74de0e.md)

    Constructs one vector from one scalar. 

* [constexpr Float4(f32 x, f32 y, f32 z, f32 w)](struct_luna_1_1_float4_1a9d9ac7f56501214f5e9d16a621e35e7c.md)

    Constructs one vector from values. 

* [bool operator==(const Float4 &v) const](struct_luna_1_1_float4_1ad8856dfa046e356cfa3af84c7df7b3ed.md)

    Compares two vectors for equality. 

* [bool operator!=(const Float4 &v) const](struct_luna_1_1_float4_1a7482716f8587458b05ccb0cd1e149222.md)

    Compares two vectors for non-equality. 

* [Float4 & operator+=(const Float4 &v)](struct_luna_1_1_float4_1aa4a62f0722143fb899a05edf643619d6.md)

    Adds this vector with one vector, and stores the result to this vector. 

* [Float4 & operator-=(const Float4 &v)](struct_luna_1_1_float4_1aae144715ce6ad450e5ad84fd7160e7a1.md)

    Subtracts this vector with one vector, and stores the result to this vector. 

* [Float4 & operator*=(const Float4 &v)](struct_luna_1_1_float4_1a0d3b4083598a02086ac7d28bcf7ca5dc.md)

    Multiplies this vector with one vector, and stores the result to this vector. 

* [Float4 & operator/=(const Float4 &v)](struct_luna_1_1_float4_1a32d36e588e57e1d8efb70c318e0f915b.md)

    Divides this vector with one vector, and stores the result to this vector. 

* [Float4 & operator+=(f32 s)](struct_luna_1_1_float4_1ad30f9245a948f94d41762a902660afb9.md)

    Adds this vector with one scalar, and stores the result to this vector. 

* [Float4 & operator-=(f32 s)](struct_luna_1_1_float4_1a059fa032990ddfff012cf9d358edcaab.md)

    Subtracts this vector with one scalar, and stores the result to this vector. 

* [Float4 & operator*=(f32 s)](struct_luna_1_1_float4_1aecb9a8d785cfddf933266e8b4c1e4962.md)

    Multiplies this vector with one scalar, and stores the result to this vector. 

* [Float4 & operator/=(f32 s)](struct_luna_1_1_float4_1ae2588d8a71a6f045f370625c07dd3553.md)

    Divides this vector with one scalar, and stores the result to this vector. 

* [Float4 operator+() const](struct_luna_1_1_float4_1aa644cf8899a7d815ba1fe0b4a8c440e6.md)

    Gets the vector as-is. 

* [Float4 operator-() const](struct_luna_1_1_float4_1aa3d6cabb51a4a13b60a658621329d011.md)

    Gets a negation of this vector. 

* [Float2 xy() const](struct_luna_1_1_float4_1a3d26cb019a0cf62ec748bdc96c792054.md)

    Gets the first two components of this vector. 

* [Float3 xyz() const](struct_luna_1_1_float4_1afbbe16970862b7e5f548749537b7c229.md)

    Gets the first three components of this vector. 

