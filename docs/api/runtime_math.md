# Math library
## Topics
* [Color operations](runtime_color.md)
* [Quaternion operations](runtime_math_quaternion.md)
* [SIMD library](runtime_math_simd.md)
* [Transform operations](runtime_math_transform.md)
* [Vectors](runtime_math_vector.md)
## Types
* [Luna::Rect](struct_luna_1_1_rect.md)

    Used to specify a 2D rectangle region using position and size. 


* [Luna::OffsetRect](struct_luna_1_1_offset_rect.md)

    Used to specify a 2D rectangle region using offsets with its container rectangle. 


* [Luna::Box](struct_luna_1_1_box.md)

    Used to specify a 3D box region using position and size. 


* [Luna::OffsetBox](struct_luna_1_1_offset_box.md)

    Used to specify a 3D box region using offsets with its container box. 


* [Luna::Float3x3](struct_luna_1_1_float3x3.md)

    3x3 matrix type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 


* [Luna::Float3x2U](struct_luna_1_1_float3x2_u.md)

    Unaligned 3x2 matrix with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 


* [Luna::Float3x3U](struct_luna_1_1_float3x3_u.md)

    Unaligned 3x3 matrix with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 


* [Luna::Float4x4](struct_luna_1_1_float4x4.md)

    4x4 matrix type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 


* [Luna::Float4x3U](struct_luna_1_1_float4x3_u.md)

    Unaligned 4x3 matrix with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 


* [Luna::Float4x4U](struct_luna_1_1_float4x4_u.md)

    Unaligned 4x4 matrix with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 


## Alias types
* [using RectI =  Rect<i32>](group___runtime_math_1gaa5b532f2f6ef76f3470a7a3c130ca343.md)

    A instanced type of [Rect](struct_luna_1_1_rect.md) that uses [i32](group___runtime_base_type_1gaec4a1429cc91fb7ff41599b263c348cc.md) as value type. 

* [using RectU =  Rect<u32>](group___runtime_math_1ga8cd4fdf14c6c1f5d9bb805b01f04f9ed.md)

    A instanced type of [Rect](struct_luna_1_1_rect.md) that uses [u32](group___runtime_base_type_1ga65cf28726f89e62ccf2f1354bc2716df.md) as value type. 

* [using RectF =  Rect<f32>](group___runtime_math_1gab414788a09e4eff0b45cbbbc0234e101.md)

    A instanced type of [Rect](struct_luna_1_1_rect.md) that uses [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) as value type. 

* [using OffsetRectI =  OffsetRect<i32>](group___runtime_math_1ga00edede5609bff78417f6145fab3af29.md)

    A instanced type of [OffsetRect](struct_luna_1_1_offset_rect.md) that uses [i32](group___runtime_base_type_1gaec4a1429cc91fb7ff41599b263c348cc.md) as value type. 

* [using OffsetRectU =  OffsetRect<u32>](group___runtime_math_1ga17244a8a7f822b65076471f0bfaddcf0.md)

    A instanced type of [OffsetRect](struct_luna_1_1_offset_rect.md) that uses [u32](group___runtime_base_type_1ga65cf28726f89e62ccf2f1354bc2716df.md) as value type. 

* [using OffsetRectF =  OffsetRect<f32>](group___runtime_math_1ga28d75b051d236f7745be3d384682ed32.md)

    A instanced type of [OffsetRect](struct_luna_1_1_offset_rect.md) that uses [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) as value type. 

* [using BoxI =  Box<i32>](group___runtime_math_1ga596254ce8bb72d10f1e14d497e9311fd.md)

    A instanced type of [Box](struct_luna_1_1_box.md) that uses [i32](group___runtime_base_type_1gaec4a1429cc91fb7ff41599b263c348cc.md) as value type. 

* [using BoxU =  Box<u32>](group___runtime_math_1gad2ad5a18b8bd4ae8f27404f11b79af53.md)

    A instanced type of [Box](struct_luna_1_1_box.md) that uses [u32](group___runtime_base_type_1ga65cf28726f89e62ccf2f1354bc2716df.md) as value type. 

* [using BoxF =  Box<f32>](group___runtime_math_1ga4bc914370aff98308e38a130b39709ff.md)

    A instanced type of [Box](struct_luna_1_1_box.md) that uses [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) as value type. 

* [using OffsetBoxI =  OffsetBox<i32>](group___runtime_math_1gac7225b81c3e578f9dee016fcd66f53b5.md)

    A instanced type of [OffsetBox](struct_luna_1_1_offset_box.md) that uses [i32](group___runtime_base_type_1gaec4a1429cc91fb7ff41599b263c348cc.md) as value type. 

* [using OffsetBoxU =  OffsetBox<u32>](group___runtime_math_1gaabba66cd7dedac457df982b4b1431561.md)

    A instanced type of [OffsetBox](struct_luna_1_1_offset_box.md) that uses [u32](group___runtime_base_type_1ga65cf28726f89e62ccf2f1354bc2716df.md) as value type. 

* [using OffsetBoxF =  OffsetBox<f32>](group___runtime_math_1ga1a974a3378044f89c505a866ca76743c.md)

    A instanced type of [OffsetBox](struct_luna_1_1_offset_box.md) that uses [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) as value type. 

## Constants
* [constexpr f32 PI](group___runtime_math_1gafce6d114b6c8b3f28b6b051d2c77a760.md)

    The constant value `pi`. 

* [constexpr f32 TWO_PI](group___runtime_math_1ga575dde3ae3140c96b822ab618fef18b7.md)

    The constant value `pi * 2.0`. 

* [constexpr f32 ONE_DIV_PI](group___runtime_math_1ga31dea32d671673a0a9a98788a16a7af3.md)

    The constant value `1.0 / pi`. 

* [constexpr f32 ONE_DIV_TWO_PI](group___runtime_math_1gaaeaef1cfa90f02bbf6a58e32b2444d76.md)

    The constant value `0.5 / pi`. 

* [constexpr f32 PI_DIV_TWO](group___runtime_math_1ga05d35bc7d317b2953f77b38a03892313.md)

    The constant value `pi / 2.0`. 

* [constexpr f32 PI_DIV_FOUR](group___runtime_math_1ga0b9bdf85d51861bec5450c3cd4e597dc.md)

    The constant value `pi / 4.0`. 

* [constexpr f32 F32_INFINITY](group___runtime_math_1ga92e79ca4e32d185971bc392297d08ddf.md)

    The INF value for f32 type. 

* [constexpr f64 F64_INFINITY](group___runtime_math_1gab4ac7a7a782d35df2f1f174899eb10b6.md)

    The INF value for f64 type. 

* [constexpr f32 F32_NAN](group___runtime_math_1ga4656aca897a6044d61422a6b0e7b8181.md)

    The NaN value for f32 type. 

* [constexpr f64 F64_NAN](group___runtime_math_1ga67bbc12d3ee15575f4360d0d1b981c56.md)

    The NaN value for f64 type. 

## Functions
* [constexpr f32 deg_to_rad(f32 degrees)](group___runtime_math_1gad2c53dfe40f543d2966b676b22215b7f.md)

    Converts degree angle to radian angle. 

* [constexpr f32 rad_to_deg(f32 radians)](group___runtime_math_1gab9cb6eaba9791a6ff572705051e245f5.md)

    Converts radian angle to degree angle. 

* [constexpr bool is_pow_of_two(_Ty n)](group___runtime_math_1gadb40e5b7beba40ffc1e6b732a92dc809.md)

    Check whether the provided number is power of two. 

* [_VTy lerp(_VTy f1, _VTy f2, _TTy t)](group___runtime_math_1gad1e29c460dec1ce5ae6007a410b9d824.md)

    Performs linear interpolation on the given values. 

* [f32 smoothstep(f32 f1, f32 f2, f32 t)](group___runtime_math_1gacb9a485e7e4b6b6d9e36a11a9265e39a.md)

    Performs smoothstep interpolation on the given values. 

* [_Ty1 clamp(_Ty1 v, _Ty2 min_v, _Ty3 max_v)](group___runtime_math_1gac0f7b129f7a4e0728696a2bca354e6d5.md)

    Clamps the value to the specified range. 

* [constexpr _Ty gcd(_Ty a, _Ty b)](group___runtime_math_1gafbb53aaee23b2bee9f08ea47cbf600c0.md)

    Calculates the Greatest Common Divisor of two numbers. 

* [Float3x3 operator+(const Float3x3 &m1, const Float3x3 &m2)](group___runtime_math_1ga41a24ee4862fb5a886d289aa088dd012.md)

    Adds two matrices. The addition is performed on every component of two matrices. 

* [Float3x3 operator+(const Float3x3 &m1, f32 s)](group___runtime_math_1ga9394d5b605c72330e97167ea94b3ca05.md)

    Adds one matrix with one scalar. The scalar will be added to every component of the matrix. 

* [Float3x3 operator+(f32 s, const Float3x3 &m1)](group___runtime_math_1ga143b63ca34a01057fc31c7c12624c3a5.md)

    Adds one matrix with one scalar. The scalar will be added to every component of the matrix. 

* [Float3x3 operator-(const Float3x3 &m1, const Float3x3 &m2)](group___runtime_math_1ga74f62a77defa536e6da88bc0b6bb8b0e.md)

    Subtracts one matrix from another matrix (m1 - m2). The subtraction is performed on every component of two matrices. 

* [Float3x3 operator-(const Float3x3 &m1, f32 s)](group___runtime_math_1ga63560b6184c0d52c359d66f3cf291ff9.md)

    Subtracts one scalar from one matrix (m1 - s). The scalar will be subtracted from every component of the matrix. 

* [Float3x3 operator-(f32 s, const Float3x3 &m1)](group___runtime_math_1gaa74f790659a25a37404cec376277a628.md)

    Subtracts one matrix from one scalar (s - m1). This behaves like creating one matrix filled with scalar `s`, then subtracting matrix `m1` from the created matrix. 

* [Float3x3 operator*(const Float3x3 &m1, const Float3x3 &m2)](group___runtime_math_1gad896031dcf9889d804e24994fc4da1d5.md)

    Multiplies two matrices. The multiplication is performed on every component of two matrices. 

* [Float3x3 operator*(const Float3x3 &m1, f32 s)](group___runtime_math_1ga644145abd7a1d048ff949ee5da4dceac.md)

    Multiplies one matrix with one scalar. The scalar will be multiplied to every component of the matrix. 

* [Float3x3 operator*(f32 s, const Float3x3 &m1)](group___runtime_math_1gad468a960b46cb8de6a8fd8753d607c2b.md)

    Multiplies one matrix with one scalar. The scalar will be multiplied to every component of the matrix. 

* [Float3x3 operator/(const Float3x3 &m1, const Float3x3 &m2)](group___runtime_math_1ga0982e291320feee847bcccbd15a1361e.md)

    Divides one matrix with another matrix (m1 / m2). The division is performed on every component of two matrices. 

* [Float3x3 operator/(const Float3x3 &m1, f32 s)](group___runtime_math_1gab1d7c2e206b499c48aa3029ade3b13ba.md)

    Divides one scalar with one matrix (m1 / s). The scalar will be divided from every component of the matrix. 

* [Float3x3 operator/(f32 s, const Float3x3 &m1)](group___runtime_math_1ga0cc506dfeb4ca5505c2a752d2b6cb3dd.md)

    Divides one matrix with one scalar (s / m1). This behaves like creating one matrix filled with scalar `s`, then dividing the created matrix with matrix `m1`. 

* [Float3 mul(const Float3 &vec, const Float3x3 &mat)](group___runtime_math_1gabbf48adca80e9634ee13bb6b6b17d00e.md)

    Performs matrix multiplication between one vector and one matrix. 

* [Float3 mul(const Float3x3 &mat, const Float3 &vec)](group___runtime_math_1ga678412bd8af84004c565c8ad07298681.md)

    Performs matrix multiplication between one matrix and one vector. 

* [Float3x3 mul(const Float3x3 &m1, const Float3x3 &m2)](group___runtime_math_1ga0e4e554d5cd5d9d21fad62772356b3fa.md)

    Performs matrix multiplication between two matrices. 

* [f32 determinant(const Float3x3 &mat)](group___runtime_math_1gac65d53221bef8dc9fba445639223af92.md)

    Computes the determinant of the specified matrix. 

* [Float3x3 transpose(const Float3x3 &mat)](group___runtime_math_1ga20eb1726f183893f6dc365c9e27a90db.md)

    Computes the transpose matrix of the specified matrix. 

* [Float3x3 inverse(const Float3x3 &mat, f32 *out_determinant=nullptr)](group___runtime_math_1gab0d9795335706f43984e0252900baa4e.md)

    Computes the inversed matrix of the specified matrix. 

* [Float4x4 operator+(const Float4x4 &m1, const Float4x4 &m2)](group___runtime_math_1gac372653fb264b55420311091562e7f68.md)

    Adds two matrices. The addition is performed on every component of two matrices. 

* [Float4x4 operator+(const Float4x4 &m1, f32 s)](group___runtime_math_1ga036400493ba1c665dc7a72cb7858278f.md)

    Adds one matrix with one scalar. The scalar will be added to every component of the matrix. 

* [Float4x4 operator+(f32 s, const Float4x4 &m1)](group___runtime_math_1gac1722a56c814fdd2c8466b89445ffab2.md)

    Adds one matrix with one scalar. The scalar will be added to every component of the matrix. 

* [Float4x4 operator-(const Float4x4 &m1, const Float4x4 &m2)](group___runtime_math_1ga038ae90b259b14377ee73af531719910.md)

    Subtracts one matrix from another matrix (m1 - m2). The subtraction is performed on every component of two matrices. 

* [Float4x4 operator-(const Float4x4 &m1, f32 s)](group___runtime_math_1gadbacd0ba085bdb88adc3a095321ab573.md)

    Subtracts one scalar from one matrix (m1 - s). The scalar will be subtracted from every component of the matrix. 

* [Float4x4 operator-(f32 s, const Float4x4 &m1)](group___runtime_math_1ga250f2483cbeb33408327978650eedc59.md)

    Subtracts one matrix from one scalar (s - m1). This behaves like creating one matrix filled with scalar `s`, then subtracting matrix `m1` from the created matrix. 

* [Float4x4 operator*(const Float4x4 &m1, const Float4x4 &m2)](group___runtime_math_1ga9154889d7a8b0215d3267cb9b8b90c80.md)

    Multiplies two matrices. The multiplication is performed on every component of two matrices. 

* [Float4x4 operator*(const Float4x4 &m1, f32 s)](group___runtime_math_1ga8f7d87f0fbd1e1d4a2226bf3941ad883.md)

    Multiplies one matrix with one scalar. The scalar will be multiplied to every component of the matrix. 

* [Float4x4 operator*(f32 s, const Float4x4 &m1)](group___runtime_math_1gaef1bacdd65129465a55c0764c1b20303.md)

    Multiplies one matrix with one scalar. The scalar will be multiplied to every component of the matrix. 

* [Float4x4 operator/(const Float4x4 &m1, const Float4x4 &m2)](group___runtime_math_1gad3bbcf7d9b608f52a1b0c5ca7dc8fb92.md)

    Divides one matrix with another matrix (m1 / m2). The division is performed on every component of two matrices. 

* [Float4x4 operator/(const Float4x4 &m1, f32 s)](group___runtime_math_1ga93b342d19cfc4d48ce9d35f1e898b5ca.md)

    Divides one scalar with one matrix (m1 / s). The scalar will be divided from every component of the matrix. 

* [Float4x4 operator/(f32 s, const Float4x4 &m1)](group___runtime_math_1ga040bf31a8351384b7258883a17b6eca3.md)

    Divides one matrix with one scalar (s / m1). This behaves like creating one matrix filled with scalar `s`, then dividing the created matrix with matrix `m1`. 

* [Float4 mul(const Float4 &vec, const Float4x4 &mat)](group___runtime_math_1ga822c0acb529c6cca425222775dd53aca.md)

    Performs matrix multiplication between one vector and one matrix. 

* [Float4 mul(const Float4x4 &mat, const Float4 &vec)](group___runtime_math_1ga84859c6d0fa9a78276b31925c2b34cd3.md)

    Performs matrix multiplication between one matrix and one vector. 

* [Float4x4 mul(const Float4x4 &mat1, const Float4x4 &mat2)](group___runtime_math_1ga499c72e985fd454382efe8a6da24ad2d.md)

    Performs matrix multiplication between two matrices. 

* [f32 determinant(const Float4x4 &mat)](group___runtime_math_1ga152d43fb81a4dfcecf64b78323e74116.md)

    Computes the determinant of the specified matrix. 

* [Float4x4 transpose(const Float4x4 &mat)](group___runtime_math_1ga0a2e2e59bfeddbc99dc9508566bc2b05.md)

    Computes the transpose matrix of the specified matrix. 

* [Float4x4 inverse(const Float4x4 &mat, f32 *out_determinant=nullptr)](group___runtime_math_1gaf2d9ae766b3a9c5cc56236748bb30dce.md)

    Computes the inversed matrix of the specified matrix. 

* [typeinfo_t float3x3_type()](group___runtime_math_1ga706751f1db935484b505f38e7c1b6dc6.md)

    Gets the type object of [Float3x3](struct_luna_1_1_float3x3.md). 

* [typeinfo_t float4x4_type()](group___runtime_math_1gaabc5aefbaa836565e8087689bd2d55c3.md)

    Gets the type object of [Float4x4](struct_luna_1_1_float4x4.md). 

