# Luna::Float4x4
4x4 matrix type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 

```c++
struct Luna::Float4x4
```

This matrix type is 16-bytes aligned and will use SIMD to accelerate matrix calculations when possible. 

## Member objects
* [Float4 r[4]](struct_luna_1_1_float4x4_1ac346f9056529f71c33cbb26cd4c06a70.md)

    The array of rows of the matrix. 

## Member functions
* [Float4x4()=default](struct_luna_1_1_float4x4_1a07aa372bb3b13f1d31f20c00b64d235b.md)

    Constructs one matrix with components uninitialized. 

* [Float4x4(const Float4x4 &)=default](struct_luna_1_1_float4x4_1a2f419de7708de0c250a16247dd575db9.md)

    Constructs one matrix by coping components from another matrix. 

* [Float4x4 & operator=(const Float4x4 &)=default](struct_luna_1_1_float4x4_1ab77facdd159c5185cb47439697031a7f.md)

    Assigns one matrix by coping components from another matrix. 

* [Float4x4(Float4x4 &&)=default](struct_luna_1_1_float4x4_1a3923152d8af5cf5b80bb5599723cdf0f.md)

    Constructs one matrix by coping components from another matrix. 

* [Float4x4 & operator=(Float4x4 &&)=default](struct_luna_1_1_float4x4_1a994d4f1de4bfe30c487326518f3cff2d.md)

    Assigns one matrix by coping components from another matrix. 

* [constexpr Float4x4(f32 m00, f32 m01, f32 m02, f32 m03, f32 m10, f32 m11, f32 m12, f32 m13, f32 m20, f32 m21, f32 m22, f32 m23, f32 m30, f32 m31, f32 m32, f32 m33)](struct_luna_1_1_float4x4_1a6bed259dc13a883bce74c67b93cd97ea.md)

    Constructs one matrix from component values. 

* [const f32 * data() const](struct_luna_1_1_float4x4_1aca402a695a2fb9fe0d9632136f551d6b.md)

    Gets the data of the matrix as one array of [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 

* [f32 * data()](struct_luna_1_1_float4x4_1a810e553b071cce584dd56318ae3985df.md)

    Gets the data of the matrix as one array of [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 

* [bool operator==(const Float4x4 &m) const](struct_luna_1_1_float4x4_1ab8959061a18b6dff4936fdf1d2292fa7.md)

    Compares two matrices for equality. 

* [bool operator!=(const Float4x4 &m) const](struct_luna_1_1_float4x4_1aa9a9a3bd6f46276b8f234cbec47b6791.md)

    Compares two matrices for non-equality. 

* [Float4x4(const Float4 &row1, const Float4 &row2, const Float4 &row3, const Float4 &row4)](struct_luna_1_1_float4x4_1af4a6c800c41f5ccae5d162ef32446a1b.md)

    Constructs one matrix from four [Float4](struct_luna_1_1_float4.md) vectors. 

* [Float4 r1() const](struct_luna_1_1_float4x4_1a3af620cd0cc93c126cadb0533c45b53b.md)

    Extracts the first row of the matrix. 

* [Float4 r2() const](struct_luna_1_1_float4x4_1a6ce0d8c96e4394e6ea3998dd3a1fa929.md)

    Extracts the second row of the matrix. 

* [Float4 r3() const](struct_luna_1_1_float4x4_1a601515c8d0585a90fea9401334e06a72.md)

    Extracts the third row of the matrix. 

* [Float4 r4() const](struct_luna_1_1_float4x4_1a6804776b876712c741e61ed508c95486.md)

    Extracts the fourth row of the matrix. 

* [Float4 c1() const](struct_luna_1_1_float4x4_1af3645c3852a24db475950a97ca5a19b2.md)

    Extracts the first column of the matrix. 

* [Float4 c2() const](struct_luna_1_1_float4x4_1ad5529231d01eef509b24de7cd4ffc243.md)

    Extracts the second column of the matrix. 

* [Float4 c3() const](struct_luna_1_1_float4x4_1a2994098a79d7a18c378046dac30ae871.md)

    Extracts the third column of the matrix. 

* [Float4 c4() const](struct_luna_1_1_float4x4_1a3f5169d4316d0e7e655e4fa64b2017cc.md)

    Extracts the fourth column of the matrix. 

* [Float4x4 operator+() const](struct_luna_1_1_float4x4_1a6ca434a3ef722b686e06bbe5eacad29c.md)

    Gets the matrix as is. 

* [Float4x4 operator-() const](struct_luna_1_1_float4x4_1a906a0ed32bbc89151dd155339e7e5de5.md)

    Gets a negative version of the matrix. 

* [Float4x4 & operator+=(const Float4x4 &mat)](struct_luna_1_1_float4x4_1ac1968bfa2cbbf0655453e100d09eea7a.md)

    Adds one matrix to this matrix. The addition is performed on every component of two matrices. 

* [Float4x4 & operator-=(const Float4x4 &mat)](struct_luna_1_1_float4x4_1a22d89540c55b69099c2e61bddd0771fa.md)

    Subtracts one matrix from this matrix. The subtraction is performed on every component of two matrices. 

* [Float4x4 & operator*=(const Float4x4 &mat)](struct_luna_1_1_float4x4_1a7533f58da1c9e6a10e9c2666698d54e0.md)

    Multiplies one matrix to this matrix. The multiplication is performed on every component of two matrices. 

* [Float4x4 & operator/=(const Float4x4 &mat)](struct_luna_1_1_float4x4_1a45d367d23698351df29264616b1cac5d.md)

    Divides one matrix from this matrix. The division is performed on every component of two matrices. 

* [Float4x4 & operator+=(f32 s)](struct_luna_1_1_float4x4_1aee3c40a4dbfede8bb5ec03949f4b1d64.md)

    Adds one scalar to this matrix. The scalar will be added to every component of the matrix. 

* [Float4x4 & operator-=(f32 s)](struct_luna_1_1_float4x4_1a8ea5345dde756382c1c5e9a0309834f2.md)

    Subtracts one scalar from this matrix. The scalar will be subtracted from every component of the matrix. 

* [Float4x4 & operator*=(f32 s)](struct_luna_1_1_float4x4_1a0c80449a8db259f735814840313abf43.md)

    Multiplies one scalar to this matrix. The scalar will be multiplied to every component of the matrix. 

* [Float4x4 & operator/=(f32 s)](struct_luna_1_1_float4x4_1a0c363b683887d78c9a044a16e77a3da4.md)

    Divides one scalar from this matrix. The scalar will be divided from every component of the matrix. 

