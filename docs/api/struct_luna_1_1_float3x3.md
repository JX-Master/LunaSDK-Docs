# Luna::Float3x3
3x3 matrix type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 

```c++
struct Luna::Float3x3
```

This matrix type is 16-bytes aligned and will use SIMD to accelerate matrix calculations when possible. 

## Member objects
* [Float3 r[3]](struct_luna_1_1_float3x3_1a025dea5773592d71ab354656c2337ef8.md)

    The array of rows of the matrix. 

## Member functions
* [Float3x3()=default](struct_luna_1_1_float3x3_1afd7f8212ea4f3485a2c2cf9afcc4e5a8.md)

    Constructs one matrix with components uninitialized. 

* [Float3x3(const Float3x3 &)=default](struct_luna_1_1_float3x3_1a598389978c147634a5c3bdbfbdd96fbe.md)

    Constructs one matrix by coping components from another matrix. 

* [Float3x3 & operator=(const Float3x3 &rhs)=default](struct_luna_1_1_float3x3_1a19a2a0811b49775f1c09c3d41c8bf2c4.md)

    Assigns one matrix by coping components from another matrix. 

* [Float3x3(Float3x3 &&rhs)=default](struct_luna_1_1_float3x3_1a5103c8c9b051f7fde08fe6a9e24ba817.md)

    Constructs one matrix by coping components from another matrix. 

* [Float3x3 & operator=(Float3x3 &&rhs)=default](struct_luna_1_1_float3x3_1ae340767e736775337f7a28aa024326b8.md)

    Assigns one matrix by coping components from another matrix. 

* [constexpr Float3x3(f32 m00, f32 m01, f32 m02, f32 m10, f32 m11, f32 m12, f32 m20, f32 m21, f32 m22)](struct_luna_1_1_float3x3_1a022483b68863f64c8eb15d79fdf9a2c6.md)

    Constructs one matrix from component values. 

* [const f32 * data() const](struct_luna_1_1_float3x3_1aca402a695a2fb9fe0d9632136f551d6b.md)

    Gets the data of the matrix as one array of [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 

* [f32 * data()](struct_luna_1_1_float3x3_1a810e553b071cce584dd56318ae3985df.md)

    Gets the data of the matrix as one array of [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 

* [bool operator==(const Float3x3 &m) const](struct_luna_1_1_float3x3_1abfc707ed9f6492320325cce26b2f7d14.md)

    Compares two matrices for equality. 

* [bool operator!=(const Float3x3 &m) const](struct_luna_1_1_float3x3_1a041a110f84d18ac63fadaca6bc41bc62.md)

    Compares two matrices for non-equality. 

* [Float3x3(const Float3 &row1, const Float3 &row2, const Float3 &row3)](struct_luna_1_1_float3x3_1aaa2f31a547d94ccef44e131d468707f3.md)

    Constructs one matrix from three [Float3](struct_luna_1_1_float3.md) vectors. 

* [Float3 r1() const](struct_luna_1_1_float3x3_1a9d2dd20f32be83a25cb4af45b1275da3.md)

    Extracts the first row of the matrix. 

* [Float3 r2() const](struct_luna_1_1_float3x3_1a80c2bc877e1b8371df24ef5a1b4d081b.md)

    Extracts the second row of the matrix. 

* [Float3 r3() const](struct_luna_1_1_float3x3_1aa7d50d7d6fe52645ad27d1d491fe3fa9.md)

    Extracts the third row of the matrix. 

* [Float3 c1() const](struct_luna_1_1_float3x3_1aa2bb58c94089d7457541603b9e85fa4c.md)

    Extracts the first column of the matrix. 

* [Float3 c2() const](struct_luna_1_1_float3x3_1aab9bb289221583feb5066d1051433a06.md)

    Extracts the second column of the matrix. 

* [Float3 c3() const](struct_luna_1_1_float3x3_1a788ffa34d2bd9f8c6deb3af93ff02818.md)

    Extracts the third column of the matrix. 

* [Float3x3 operator+() const](struct_luna_1_1_float3x3_1a467177880602835cefeb389584991118.md)

    Gets the matrix as is. 

* [Float3x3 operator-() const](struct_luna_1_1_float3x3_1ad234cac42c98a69fe7277ecb56f8766d.md)

    Gets a negative version of the matrix. 

* [Float3x3 & operator+=(const Float3x3 &mat)](struct_luna_1_1_float3x3_1ad7d7803afff10c50d01fcbeb33e7ebe0.md)

    Adds one matrix to this matrix. The addition is performed on every component of two matrices. 

* [Float3x3 & operator-=(const Float3x3 &mat)](struct_luna_1_1_float3x3_1adeb3089df98466704604f2edb4d3b814.md)

    Subtracts one matrix from this matrix. The subtraction is performed on every component of two matrices. 

* [Float3x3 & operator*=(const Float3x3 &mat)](struct_luna_1_1_float3x3_1a603db7789c167353c47ed80fcdbf0bc3.md)

    Multiplies one matrix to this matrix. The multiplication is performed on every component of two matrices. 

* [Float3x3 & operator/=(const Float3x3 &mat)](struct_luna_1_1_float3x3_1a43c052d3065c79e0aad5cb8af6ab057c.md)

    Divides one matrix from this matrix. The division is performed on every component of two matrices. 

* [Float3x3 & operator+=(f32 s)](struct_luna_1_1_float3x3_1a6a55156bcbfd814bc44c8e1fbe06058e.md)

    Adds one scalar to this matrix. The scalar will be added to every component of the matrix. 

* [Float3x3 & operator-=(f32 s)](struct_luna_1_1_float3x3_1aff4576af39c467ad4575853746770e7f.md)

    Subtracts one scalar from this matrix. The scalar will be subtracted from every component of the matrix. 

* [Float3x3 & operator*=(f32 s)](struct_luna_1_1_float3x3_1acb64aea10ef021ee25f3c1927f3a8977.md)

    Multiplies one scalar to this matrix. The scalar will be multiplied to every component of the matrix. 

* [Float3x3 & operator/=(f32 s)](struct_luna_1_1_float3x3_1a2ac31163c52eaa1cbcbe1e469ed731fa.md)

    Divides one scalar from this matrix. The scalar will be divided from every component of the matrix. 

