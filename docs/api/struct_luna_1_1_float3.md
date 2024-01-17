# Luna::Float3
3D vector type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 

```c++
struct Luna::Float3
```

This vector type is 16-bytes aligned and will use SIMD to accelerate vector calculations when possible. 

## Member objects
* [f32 x](struct_luna_1_1_float3_1a6b05cac69c0301ab972c27ce208373be.md)

    The fist component of the vector. 

* [f32 y](struct_luna_1_1_float3_1ab7291adeb8828a0cba3aedf332c2053d.md)

    The second component of the vector. 

* [f32 z](struct_luna_1_1_float3_1aac280fcf3516d20b5e3dec5fa770ac50.md)

    The third component of the vector. 

* [f32 m[3]](struct_luna_1_1_float3_1a22adc523a97266b8d30a1ee6fdf24920.md)

    The array of components. 

## Member functions
* [Float3()=default](struct_luna_1_1_float3_1a22f630ee6af53afcc8d5bdddf52f94fa.md)

    Constructs one vector with components uninitialized. 

* [Float3(const Float3 &)=default](struct_luna_1_1_float3_1ab5e25248c6e3954e88cffa3a05ed7ef1.md)

    Constructs one vector by coping components from another vector. 

* [Float3 & operator=(const Float3 &)=default](struct_luna_1_1_float3_1adbc90d57479f368fa10e690d7ebb6b17.md)

    Assigns one vector by coping components from another vector. 

* [Float3(Float3 &&)=default](struct_luna_1_1_float3_1adc95db3846299f5b63c5551097257222.md)

    Constructs one vector by coping components from another vector. 

* [Float3 & operator=(Float3 &&)=default](struct_luna_1_1_float3_1aef5a23b61d513c21955229705bd4a5df.md)

    Assigns one vector by coping components from another vector. 

* [constexpr Float3(f32 s)](struct_luna_1_1_float3_1a70ca5359562ece0004a34605eaf3b95d.md)

    Constructs one vector from one scalar. 

* [constexpr Float3(f32 x, f32 y, f32 z)](struct_luna_1_1_float3_1ab61ff04894017cbc51c209b1fc881d9e.md)

    Constructs one vector from values. 

* [bool operator==(const Float3 &v) const](struct_luna_1_1_float3_1a4189051c755d667ac83d648bfd9ea6e5.md)

    Compares two vectors for equality. 

* [bool operator!=(const Float3 &v) const](struct_luna_1_1_float3_1aa2ed30e30c7989a1e720a3771a8a3e19.md)

    Compares two vectors for non-equality. 

* [Float3 & operator+=(const Float3 &v)](struct_luna_1_1_float3_1a722f64ac4535d31fa3eda8af88286144.md)

    Adds this vector with one vector, and stores the result to this vector. 

* [Float3 & operator-=(const Float3 &v)](struct_luna_1_1_float3_1abb3a6978dc7feb9ff8768acf47a7fb4d.md)

    Subtracts this vector with one vector, and stores the result to this vector. 

* [Float3 & operator*=(const Float3 &v)](struct_luna_1_1_float3_1ac0793284e6e19c1709de18858ac31a3c.md)

    Multiplies this vector with one vector, and stores the result to this vector. 

* [Float3 & operator/=(const Float3 &v)](struct_luna_1_1_float3_1ae1e1cb9f9ea60856dc51bf2006de366c.md)

    Divides this vector with one vector, and stores the result to this vector. 

* [Float3 & operator+=(f32 s)](struct_luna_1_1_float3_1a5b027638699cd01bcab6706043981f19.md)

    Adds this vector with one scalar, and stores the result to this vector. 

* [Float3 & operator-=(f32 s)](struct_luna_1_1_float3_1aad66235dfe2902c6bc1e43baa34e0f8f.md)

    Subtracts this vector with one scalar, and stores the result to this vector. 

* [Float3 & operator*=(f32 s)](struct_luna_1_1_float3_1ac779f2086781827cc50f9c036764f67d.md)

    Multiplies this vector with one scalar, and stores the result to this vector. 

* [Float3 & operator/=(f32 s)](struct_luna_1_1_float3_1a04bb52c5e8cb4eccd025110980a16a9d.md)

    Divides this vector with one scalar, and stores the result to this vector. 

* [Float3 operator+() const](struct_luna_1_1_float3_1ad5d3ec1a7506ea754b02e5f01553e2c7.md)

    Gets the vector as-is. 

* [Float3 operator-() const](struct_luna_1_1_float3_1aba367c24696c2f30211446d5fcd87379.md)

    Gets a negation of this vector. 

* [Float2 xy() const](struct_luna_1_1_float3_1a3d26cb019a0cf62ec748bdc96c792054.md)

    Gets the first two components of this vector. 

