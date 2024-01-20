# SIMD library
## Types
* [Luna::Simd::float3x4](struct_luna_1_1_simd_1_1float3x4.md)

    Represents one SIMD matrix type with 12 (3x4) packed single-precision (32-bit) floating-point elements. Based on the implementation, the matrix may be stored using two 256-bits registers (AVX), or four 128-bits registers (SSEn / Neon). 


* [Luna::Simd::float4x4](struct_luna_1_1_simd_1_1float4x4.md)

    Represents one SIMD matrix type with 16 (4x4) packed single-precision (32-bit) floating-point elements. Based on the implementation, the matrix may be stored using two 256-bits registers (AVX), or four 128-bits registers (SSEn / Neon). 


## Functions
* [float4 casti_f4(int4 a)](group___runtime_math_simd_1gaeba45c41cbd8009a1d8d437c41ca4ca3.md)

    Reinterprets SIMD varaible of type `int4` to type `float4` without changing the data of the varaible. 

* [int4 castf_i4(float4 a)](group___runtime_math_simd_1gaff75e25198b1ee433671d4cb91bd08f7.md)

    Reinterprets SIMD varaible of type `float4` to type `int4` without changing the data of the varaible. 

* [float4 load_f2(f32 const *mem_addr)](group___runtime_math_simd_1gaa16aac2615c725b749cc4633e155ec97.md)

    Loads 64-bits (composed of 2 packed single-precision (32-bit) floating-point elements) from memory into the first two elements of `dst`. The rest 2 elements are filled with 0. 

* [float4 load_f4(f32 const *mem_addr)](group___runtime_math_simd_1ga34c5e90866544514ff3d63232417b291.md)

    Loads 128-bits (composed of 4 packed single-precision (32-bit) floating-point elements) from memory into `dst`. 

* [void store_f2(f32 *mem_addr, float4 a)](group___runtime_math_simd_1ga765d7f194dccbeebf8423915a236669a.md)

    Stores the lower 2 single-precision (32-bit) floating-point elements from `a` into memory. 

* [void store_f4(f32 *mem_addr, float4 a)](group___runtime_math_simd_1gae6cca4f2e19d8c2db6e969ea50ce4df2.md)

    Stores 128-bits (composed of 4 packed single-precision (32-bit) floating-point elements) from `a` into memory. 

* [float4 set_f4(f32 e0, f32 e1, f32 e2, f32 e3)](group___runtime_math_simd_1ga6fe29a5ae0b7bef26fa3a1a4617a433b.md)

    Sets packed single-precision (32-bit) floating-point elements in `dst` with the supplied values. 

* [int4 set_i4(i32 e0, i32 e1, i32 e2, i32 e3)](group___runtime_math_simd_1ga12f402bb81b069ddb27ac871a741c0fb.md)

    Sets packed 32-bit integers in `dst` with the supplied values. 

* [float4 setzero_f4()](group___runtime_math_simd_1ga6f7d72cc8754b57f6e1f7d9ed0b6b2a6.md)

    Returns vector of type `float4` with all elements set to zero. 

* [float4 dup_f4(f32 e0)](group___runtime_math_simd_1ga095ea5a2b5d180feaf56ddcca7e5993a.md)

    Broadcasts single-precision (32-bit) floating-point value `e0` to all elements of `dst`. 

* [f32 getx_f4(float4 a)](group___runtime_math_simd_1gac27bfcbdd8c79b0089d4ba0148c9bd7b.md)

    Stores the first single-precision (32-bit) floating-point element from `a` into `dst`. 

* [float4 setw_f4(float4 a, f32 b)](group___runtime_math_simd_1ga6d0ae8dc8cdf91c2649e4b23065edda0.md)

    Replaces the forth element of `a` with `b`, and stores the results in `dst`. 

* [float4 dupx_f4(float4 a)](group___runtime_math_simd_1ga003f42dc5548484e29bd46503611f64c.md)

    Broadcasts the first element of `a` to every element of `dst`. 

* [float4 dupy_f4(float4 a)](group___runtime_math_simd_1ga1937eb9d5e48a503e1abf4cedf8e5915.md)

    Broadcasts the second element of `a` to every element of `dst`. 

* [float4 dupz_f4(float4 a)](group___runtime_math_simd_1ga484b753d428f90e8e2a02cf01c0dd938.md)

    Broadcasts the third element of `a` to every element of `dst`. 

* [float4 dupw_f4(float4 a)](group___runtime_math_simd_1gadf181750b7a4d015d20a0e47e16698a4.md)

    Broadcasts the forth element of `a` to every element of `dst`. 

* [int4 cmpeq_f4(float4 a, float4 b)](group___runtime_math_simd_1ga934b303e16fbc83806b072bb19ff0142.md)

    Compares packed single-precision (32-bit) floating-point elements in `a` and `b` for equality, and stores the results in `dst`. 

* [int4 cmpneq_f4(float4 a, float4 b)](group___runtime_math_simd_1ga7eea793c8be2917d1dfd7b87cee4c49d.md)

    Compares packed single-precision (32-bit) floating-point elements in `a` and `b` for not-equal, and stores the results in `dst`. 

* [int4 cmpgt_f4(float4 a, float4 b)](group___runtime_math_simd_1ga0adb253c26d9e679967d4fa1b63ba3d1.md)

    Compares packed single-precision (32-bit) floating-point elements in `a` and `b` for greater-than, and stores the results in `dst`. 

* [int4 cmplt_f4(float4 a, float4 b)](group___runtime_math_simd_1gaa0c92da2d033831560843196f28544ce.md)

    Compares packed single-precision (32-bit) floating-point elements in `a` and `b` for less-than, and stores the results in `dst`. 

* [int4 cmpge_f4(float4 a, float4 b)](group___runtime_math_simd_1ga98173a56bccb1d6edf67729aac87422d.md)

    Compares packed single-precision (32-bit) floating-point elements in `a` and `b` for greater-than-or-equal, and stores the results in dst. 

* [int4 cmple_f4(float4 a, float4 b)](group___runtime_math_simd_1gaf6c100ac91cdffc8d8b490e1193e1eba.md)

    Compares packed single-precision (32-bit) floating-point elements in `a` and `b` for less-than-or-equal, and stores the results in dst. 

* [i32 maskint_i4(int4 a)](group___runtime_math_simd_1gae9ada5c9a40abfe8bc3a4d809c37c692.md)

    Converts the comparison result mask to one 32-bit integer. 

* [float4 add_f4(float4 a, float4 b)](group___runtime_math_simd_1ga2a885e6de9dfbd83cc5a897bc8b6e37e.md)

    Adds packed single-precision (32-bit) floating-point elements in `a` and `b`, and stores the results in `dst`. 

* [float4 sub_f4(float4 a, float4 b)](group___runtime_math_simd_1ga9f253aa40995ad21ef9e197642f6dda8.md)

    Subtracts packed single-precision (32-bit) floating-point elements in `a` and `b`, and stores the results in `dst`. 

* [float4 mul_f4(float4 a, float4 b)](group___runtime_math_simd_1ga2e897627d94e9bc921f16008d3085f06.md)

    Multiplies packed single-precision (32-bit) floating-point elements in `a` and `b`, and stores the results in `dst`. 

* [float4 div_f4(float4 a, float4 b)](group___runtime_math_simd_1gaf40f006a4eaf5ecff6edac3f6a125a64.md)

    Divides packed single-precision (32-bit) floating-point elements in a by packed elements in b, and stores the results in dst. 

* [float4 scale_f4(float4 a, f32 b)](group___runtime_math_simd_1ga949a7b6a06c102c271731207a6bff34f.md)

    Scales packed single-precision (32-bit) floating-point elements in `a` using one single-precision (32-bit) floating-point element `b`, and stores the results in `dst`. 

* [float4 muladd_f4(float4 a, float4 b, float4 c)](group___runtime_math_simd_1gad096930eef3c356ff241de6ac14c21ba.md)

    Multiply packed single-precision (32-bit) floating-point elements in `a` and `b`, add the intermediate result to packed elements in `c`, and store the results in `dst`. 

* [float4 negmuladd_f4(float4 a, float4 b, float4 c)](group___runtime_math_simd_1gad5ab9e11eed1549b0b5538f326c8d3dd.md)

    Multiply packed single-precision (32-bit) floating-point elements in `a` and `b`, add the negated intermediate result to packed elements in `c`, and store the results in dst. 

* [float4 scaleadd_f4(float4 a, f32 b, float4 c)](group___runtime_math_simd_1ga3999cd272f16fc26720dba559d102ec5.md)

    Scales packed single-precision (32-bit) floating-point elements in `a` using one single-precision (32-bit) floating-point element `b`, add the intermediate result to packed elements in `c`, and stores the results in `dst`. 

* [float4 sqrt_f4(float4 a)](group___runtime_math_simd_1gae574b820499b1e3b194271b9b1057d4d.md)

    Computes the square root of packed single-precision (32-bit) floating-point elements in `a`, and stores the results in `dst`. 

* [float4 rsqrtest_f4(float4 a)](group___runtime_math_simd_1ga579863b7a690612bdb6268ce1ebc4199.md)

    Computes the approximate reciprocal square root of packed single-precision (32-bit) floating-point elements in `a`, and stores the results in `dst`. SSE specific: The maximum relative error for this approximation is less than 1.5*2^-12. 

* [float4 rsqrt_f4(float4 a)](group___runtime_math_simd_1ga93aa0859aab5566f26d9b39cdb822779.md)

    Computes the reciprocal square root of packed single-precision (32-bit) floating-point elements in `a`, and stores the results in `dst`. 

* [float4 max_f4(float4 a, float4 b)](group___runtime_math_simd_1gab6fcdf27e6c86224b7a1ecba3a04b496.md)

    Compare packed single-precision (32-bit) floating-point elements in `a` and `b`, and store packed maximum values in `dst`. SSE specific: `dst` does not follow the IEEE Standard for Floating - Point Arithmetic(IEEE 754) maximum value when inputs are NaN or signed - zero values. 

* [float4 min_f4(float4 a, float4 b)](group___runtime_math_simd_1ga9d3db86a393321474fb7abec8490e876.md)

    Compare packed single-precision (32-bit) floating-point elements in `a` and `b`, and store packed minimum values in `dst`. SSE specific: `dst` does not follow the IEEE Standard for Floating - Point Arithmetic(IEEE 754) minimum value when inputs are NaN or signed - zero values. 

* [int4 and_i4(int4 a, int4 b)](group___runtime_math_simd_1ga60b15313668eea87792f152d79c2c198.md)

    Computes the bitwise AND of every bit in `a` and `b`, and stores the results in `dst`. 

* [int4 or_i4(int4 a, int4 b)](group___runtime_math_simd_1ga7e724e3ab4852ee1f52bfad339614c3a.md)

    Computes the bitwise OR of every bit in `a` and `b`, and stores the results in `dst`. 

* [f32 dot2_f4(float4 a, float4 b)](group___runtime_math_simd_1ga4fd7c4e031acdf7d29a553994eaafa30.md)

    Computes the dot product on the first two elements of `a` and `b`, and stores the result in `dst`. 

* [f32 dot3_f4(float4 a, float4 b)](group___runtime_math_simd_1ga37b7f375c85040da1479774245e0ed27.md)

    Computes the dot product on the first three elements of `a` and `b`, and stores the result in `dst`. 

* [f32 dot4_f4(float4 a, float4 b)](group___runtime_math_simd_1ga1ec75bc6d5473801bc053f4d0831f307.md)

    Computes the dot product on elements of `a` and `b`, and stores the result in `dst`. 

* [float4 dot2v_f4(float4 a, float4 b)](group___runtime_math_simd_1ga5396fed3f45478a42411433e7b426629.md)

    Computes the dot product on the first two elements of `a` and `b`, and stores the result in each element of `dst`. 

* [float4 dot3v_f4(float4 a, float4 b)](group___runtime_math_simd_1ga6e34d8c19c95624c048c0a89b3c47c27.md)

    Computes the dot product on the first three elements of `a` and `b`, and stores the result in each element of `dst`. 

* [float4 dot4v_f4(float4 a, float4 b)](group___runtime_math_simd_1ga72a0c28a566958301ff2b711ea50b9be.md)

    Computes the dot product on elements of `a` and `b`, and stores the result in each element of `dst`. 

* [float4 cross2_f4(float4 a, float4 b)](group___runtime_math_simd_1ga8f6180179e7ab93f662554ba1b587bd8.md)

    Computes the cross product on the first two elements of `a` and `b`, and stores the result in `dst`. 

* [float4 cross3_f4(float4 a, float4 b)](group___runtime_math_simd_1ga3ba140ea3f6ab608efda15c16b729a34.md)

    Computes the cross product on the first three elements of `a` and `b`, and stores the result in each element of `dst`. 

* [float4 cross4_f4(float4 a, float4 b, float4 c)](group___runtime_math_simd_1ga522a9d61fc8105c2851eeb6c03b09744.md)

    Computes the cross product on elements of `a`, `b` and `c`, and stores the result in each element of `dst`. 

* [float4 normalize2_f4(float4 a)](group___runtime_math_simd_1gadd3e99bad6fcd31a354408ef0af1eaed.md)

    Normalizes the first two elements of `a`, and stores the result in `dst`. 

* [float4 normalize3_f4(float4 a)](group___runtime_math_simd_1ga88fb57853009a23d5af5bff0df0619ac.md)

    Normalizes the first three elements of `a`, and stores the result in `dst`. 

* [float4 normalize4_f4(float4 a)](group___runtime_math_simd_1ga275146ac721ff87f1467daca08230f25.md)

    Normalizes elements of `a`, and stores the result in `dst`. 

* [float4 reflect2_f4(float4 i, float4 n)](group___runtime_math_simd_1ga6d67cce2953e229a49e7c9fc1c018816.md)

    Performs reflection operation based on the first two elements of `i` (incident vector) and `n`(normal vector), and stores the refected vector in `dst`. 

* [float4 reflect3_f4(float4 i, float4 n)](group___runtime_math_simd_1ga80f9a9aab3b6dc347fd0001a107e71f1.md)

    Performs reflection operation based on the first three elements of `i` (incident vector) and `n`(normal vector), and stores the refected vector in `dst`. 

* [float4 reflect4_f4(float4 i, float4 n)](group___runtime_math_simd_1ga3dc0be29aea0e1dcb3414b6fa8aaa03c.md)

    Performs reflection operation based on elements of `i` (incident vector) and `n`(normal vector), and stores the refected vector in `dst`. 

* [float4 refract2_f4(float4 i, float4 n, f32 index)](group___runtime_math_simd_1ga902430183deb8111c0af22d4cb2cb65d.md)

    Performs refraction operation based on the first two elements of `i` (incident vector), `n`(normal vector) and the scalar value `index` (refraction index), and stores the refected vector in `dst`. 

* [float4 refract3_f4(float4 i, float4 n, f32 index)](group___runtime_math_simd_1gac27a1a0e6d6461575e435c992ded8a84.md)

    Performs refraction operation based on the first three elements of `i` (incident vector), `n`(normal vector) and the scalar value `index` (refraction index), and stores the refected vector in `dst`. 

* [float4 refract4_f4(float4 i, float4 n, f32 index)](group___runtime_math_simd_1gaad60aa5e0b86fb6783689ff4455f371b.md)

    Performs refraction operation based on elements of `i` (incident vector), `n`(normal vector) and the scalar value `index` (refraction index), and stores the refected vector in `dst`. 

* [float4 lerp_f4(float4 a, float4 b, f32 t)](group___runtime_math_simd_1ga0a4dc71745e3a40a59b94e3bf6872029.md)

    Computes linear interpolation on packed single-precision (32-bit) floating-point elements in `a` and `b` using the single-precision (32-bit) floating-point value `t`, and stores the results in `dst`. 

* [float4 lerpv_f4(float4 a, float4 b, float4 t)](group___runtime_math_simd_1ga3ab9982511a996fff0e1e81574870feb.md)

    Computes linear interpolation on packed single-precision (32-bit) floating-point elements in `a` and `b` using the corresponding packed single-precision (32-bit) floating-point element in `t`, and stores the results in `dst`. 

* [float4 barycentric_f4(float4 a, float4 b, float4 c, f32 f, f32 g)](group___runtime_math_simd_1ga8137dc80423e827443f65bb283927654.md)

    Computes barycentric interpolation on packed single-precision (32-bit) floating-point elements in `a`, `b` and `c` using the single-precision (32-bit) floating-point values `f` and `g`, and stores the results in `dst`. 

* [float4 catmull_rom_f4(float4 a, float4 b, float4 c, float4 d, f32 t)](group___runtime_math_simd_1ga0fb3a92548b027ae67011771998737f2.md)

    Computes Catmull-Rom spline interpolation on packed single-precision (32-bit) floating-point elements in `a`, `b`, `c` and `d` using the single-precision (32-bit) floating-point value `t`, and stores the results in `dst`. 

* [float4 hermite_f4(float4 v0, float4 t0, float4 v1, float4 t1, f32 t)](group___runtime_math_simd_1ga1adafbac2fced6f32462e1d2a7c7b83f.md)

    Computes Hermite spline interpolation on packed single-precision (32-bit) floating-point elements in `v0`, `t0`, `v1` and `t1` using the single-precision (32-bit) floating-point value `t`, and stores the results in `dst`. 

* [float4 permute_f4(float4 a)](group___runtime_math_simd_1ga49dbae2d7cea089e24cc307b2b156d69.md)

    Shuffles single-precision (32-bit) floating-point elements in `a` based on the control parameter `_SelectX`, `_SelectY`, `_SelectZ` and `_SelectW`, and stores the results in `dst`. 

* [float4 select_f4(float4 a, float4 b)](group___runtime_math_simd_1gaf560df485472210f46d5599aa7b51171.md)

    Performs a per-component selection between `a` and `b` based on the control parameter `_SelectX`, `_SelectY`, `_SelectZ` and `_SelectW`, and stores the results in `dst`. 

* [float4 permute2_f4(float4 a, float4 b)](group___runtime_math_simd_1gad18bf22d600432f0edcf12977731a774.md)

    Shuffles single-precision (32-bit) floating-point elements in `a` and `b` based on the control parameter `_SelectX`, `_SelectY`, `_SelectZ` and `_SelectW`, and stores the results in `dst`. 

* [float3x4 load_f3x4(f32 const *mem_addr)](group___runtime_math_simd_1ga4a88cf6b25c7f0646ae05377b1e18c4d.md)

    Loads 12 packed single-precision (32-bit) floating-point elements from `mem_addr` to `dst`. The highest 4 packed single-precision (32-bit) floating-point elements are uninitialized. 

* [float4x4 load_f4x4(f32 const *mem_addr)](group___runtime_math_simd_1ga36b4b1ccc273d39da983789610bfc72e.md)

    Loads 16 packed single-precision (32-bit) floating-point elements from `mem_addr` to `dst`. `mem_addr` must be aligned on a 16-byte boundary or a general-protection exception may be generated. 

* [float4x4 setf4_f4x4(float4 r0, float4 r1, float4 r2, float4 r3)](group___runtime_math_simd_1ga3871ab0ed273218e85e8514df048963b.md)

    Creates one 4x4 matrix by loading four vectors, and stores the result in `dst`. 

* [void store_f3x4(f32 *mem_addr, float3x4 m)](group___runtime_math_simd_1gaff3c751d6ca27d277b180bd54c50cb0a.md)

    Stores the first 12 packed single-precision (32-bit) floating-point elements from `m` to `dst`. `mem_addr` must be aligned on a 16-byte boundary or a general-protection exception may be generated. 

* [void store_f4x4(f32 *mem_addr, float4x4 m)](group___runtime_math_simd_1ga8f48a5333baff26a19542c2e9cd8c5cc.md)

    Stores packed single-precision (32-bit) floating-point elements from `m` to `dst`. `mem_addr` must be aligned on a 16-byte boundary or a general-protection exception may be generated. 

* [float4x4 setzero_f4x4()](group___runtime_math_simd_1gaa5923af450c0c6e3a2a85bee080770c8.md)

    Returns matrix of type `float4x4` with all elements set to zero. 

* [float3x4 matmul_f3x3(float3x4 a, float3x4 b)](group___runtime_math_simd_1ga905ea04898bc2c1676884abaf610830f.md)

    Performs 3x3 matrix multiplication on `a` and `b`, and stores the result in `dst`. 

* [float4x4 matmul_f4x4(float4x4 a, float4x4 b)](group___runtime_math_simd_1gae278d60e69b3d0feeb8f7f8028b90e69.md)

    Performs 4x4 matrix multiplication on `a` and `b`, and stores the result in `dst`. 

* [float4x4 transpose_f4x4(float4x4 a)](group___runtime_math_simd_1ga388fc72277ccee04ec9f375208e2895a.md)

    Performs matrix transpose on `a`, and stores the result in `dst`. 

* [f32 determinant_f3x3(float3x4 a)](group___runtime_math_simd_1ga8721a156d8bc0b802e7a0e606ea61f77.md)

    Computes the determinant of the 3x3 matrix `a`, and stores the result in `dst`. 

* [float4 determinantv_f3x3(float3x4 a)](group___runtime_math_simd_1gad5240bef03d00a9fb9e0046d7d275860.md)

    Computes the determinant of the 3x3 matrix `a`, and stores the result in every element of `dst`. 

* [float3x4 inverse_f3x3(float3x4 a, f32 *out_determinant)](group___runtime_math_simd_1ga453c621e929d8cff8372ec3d0695c975.md)

    Computes the determinant and the inverse matrix of `a`, stores the determinant in `out_determinant`, and stores the inverse matrix in `dst`. 

* [f32 determinant_f4x4(float4x4 a)](group___runtime_math_simd_1ga5c7280e25a6c39f2411f1a6b1a6125f3.md)

    Calculates the determinant of matrix `a`, and stores the result in `dst`. 

* [float4 determinantv_f4x4(float4x4 a)](group___runtime_math_simd_1gae8a6101573a2dd74028b625a6b6cc0c5.md)

    Calculates the determinant of matrix `a`, and stores the result in every element of `dst`. 

* [float4x4 inverse_f4x4(float4x4 a, f32 *out_determinant)](group___runtime_math_simd_1ga611bda8e65a2a1ec09359090888925b1.md)

    Computes the determinant and the inverse matrix of `a`, stores the determinant in `out_determinant`, and stores the inverse matrix in `dst`. 

* [float4 round_f4(float4 a)](group___runtime_math_simd_1ga2ce40b16a7f21a61b21f4baa1de9657f.md)

    Rounds each component of `a` to the nearest even integer. 

* [float4 modangle_f4(float4 a)](group___runtime_math_simd_1gad14bc4ff7821a67e43f73c530d00e4e1.md)

    Computes the per-component angle modulo 2PI for `a`, and stores the results in `dst`. The angle is expressed in radians. The result is rounded in [-PI, PI]. 

* [float4 sin_f4(float4 a)](group___runtime_math_simd_1ga019baf87ae51b1f08625a3688fd6571a.md)

    Computes the sine of packed single-precision (32-bit) floating-point elements in `a` expressed in radians, and stores the results in `dst`. 

* [float4 cos_f4(float4 a)](group___runtime_math_simd_1gaa405c0cecdbbd0a6070e76c7c2f9dd4d.md)

    Computes the cosine of packed single-precision (32-bit) floating-point elements in `a` expressed in radians, and stores the results in `dst`. 

* [float4 sincos_f4(float4 &out_cos, float4 a)](group___runtime_math_simd_1ga8353ffe0bd77e559d5e141ab7d6e422c.md)

    Computes the sine and cosine of packed single-precision (32-bit) floating-point elements in `a` expressed in radians, and stores the results in `dst` and `out_cos`. 

* [float4 mulquat_f4(float4 a, float4 b)](group___runtime_math_simd_1ga1d0c72657ccf1a16fbaf52ff3e98aeff.md)

    Multiplies two quaternion `a` and `b`, and stores the result in `dst`. 

* [float4 quatinverse_f4(float4 a)](group___runtime_math_simd_1gad3dd701f15a6efbd17bd39b4955c7a70.md)

    Inverts the quaternion `a`, and stores the result in `dst`. 

* [float4 quatnormalangle_f4(float4 n, f32 a)](group___runtime_math_simd_1gabc8b0777809a7d66009c6a3687ea5ce4.md)

    Computes one rotation quaternion based on the given normal `a` and one angle `a`, and stores the result quaternion in `dst`. 

* [float4 quateulerangles_f4(float4 a)](group___runtime_math_simd_1gad73ef75e29746bacc408f458eb418a4a.md)

    Computes a rotation quaternion based on a vector containing the Euler angles (pitch, yaw, and roll), and stores the result in `dst`. 

* [float4 quatlerp_f4(float4 a, float4 b, f32 t)](group___runtime_math_simd_1gaaff5564ee8a58d8e625c34912776496a.md)

    Interpolates between two unit quaternions `a` and `b` using linear interpolation, and stores the result in `dst`. 

* [float4 quatslerp_f4(float4 a, float4 b, f32 t)](group___runtime_math_simd_1ga375d007641809330162a975058150333.md)

    Interpolates between two unit quaternions `a` and `b` using spherical linear interpolation, and stores the result in `dst`. 

* [float3x4 transform2d_f3x4(float4 translation, f32 rotation, float4 scaling)](group___runtime_math_simd_1gacc44a27f246ec5b46b3725d72e8bc41b.md)

    Builds a 2D affine matrix from translation, rotation and scaling. 

* [float3x4 transform2d_translation_f3x4(float4 translation)](group___runtime_math_simd_1gaa7e9203ee0c24952577b435644f83623.md)

    Builds a 2D affine matrix from translation. 

* [float3x4 transform2d_rotation_f3x4(f32 rotation)](group___runtime_math_simd_1ga6c81f1c552b38f269d46b3acc4dbd6fa.md)

    Builds a 2D affine matrix from roation. 

* [float3x4 transform2d_scaling_f3x4(float4 scaling)](group___runtime_math_simd_1gac04609318b614b83cfe94bc12bb39caa.md)

    Builds a 2D affine matrix from scaling. 

* [float4x4 transform3d_f4x4(float4 translation, float4 rotation_quaternion, float4 scaling)](group___runtime_math_simd_1ga33e5d9338b2d537a664d5cf588afd5b2.md)

    Builds a 3D affine matrix from translation, rotation and scaling. 

* [float4x4 transform3d_translation_f4x4(float4 translation)](group___runtime_math_simd_1gaa7add3e664580b98737d6b89f633a3fd.md)

    Builds a 3D affine matrix from translation. 

* [float4x4 transform3d_rotation_quaternion_f4x4(float4 quaternion)](group___runtime_math_simd_1gaff3c5730333a685b346be2470b5f1eb7.md)

    Builds a 3D affine matrix from rotation represented by one quaternion. 

* [float4x4 transform3d_rotation_x_f4x4(f32 rotation)](group___runtime_math_simd_1ga291bbac107c57dc9b80496567bfbf256.md)

    Builds a 3D affine matrix from rotation along X axis. 

* [float4x4 transform3d_rotation_y_f4x4(f32 rotation)](group___runtime_math_simd_1ga05b8cd312eadb6dbb6f13c02edf4cfe1.md)

    Builds a 3D affine matrix from rotation along Y axis. 

* [float4x4 transform3d_rotation_z_f4x4(f32 rotation)](group___runtime_math_simd_1ga16f68c25ad52fa3087b9fd5d26c7b521.md)

    Builds a 3D affine matrix from rotation along Z axis. 

* [float4x4 transform3d_rotation_normal_angle_f4x4(float4 normal, f32 angle)](group___runtime_math_simd_1gace0a39ac7306d9103d10bf163a7c70bb.md)

    Builds a 3D affine matrix from rotation represented by rotation axis and rotation angle. 

* [float4x4 transform3d_rotation_euler_angles_f4x4(float4 pitch_yaw_roll)](group___runtime_math_simd_1ga491aced085da8908ed39c75c1e5e05e9.md)

    Builds a 3D affine matrix from rotation represented by euler angles (pitch, yaw, roll). 

* [float4x4 transform3d_scaling_f4x4(float4 scaling)](group___runtime_math_simd_1ga0e98263c36bb78a5a60d0517c4dc58ec.md)

    Builds a 3D affine matrix from scaling. 

* [float4x4 transform3d_look_to_f4x4(float4 eye, float4 eyedir, float4 updir)](group___runtime_math_simd_1gac70ec409bda6a2c0701a9d87acdfcc7b.md)

    Creates one affine matrix that trnasforms points and directions in world space to view space. `eyedir` and `updir` must be normalized. 

