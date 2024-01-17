# Luna::Float4x3U
Unaligned 4x3 matrix with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 

```c++
struct Luna::Float4x3U
```

This can be used to store 4x4 affine matrices since the fourth column is always (0, 0, 0, 1), which can be removed to reduce memory size. 

## Member objects
* [Float3U r[4]](struct_luna_1_1_float4x3_u_1abaa9e7d306e16a29b0206bce9acc0cfc.md)

    The array of rows of the matrix. 

## Member functions
* [Float4x3U()=default](struct_luna_1_1_float4x3_u_1ab4d61a9a09f431d448b804b7964849de.md)

    Constructs one matrix with components uninitialized. 

* [Float4x3U(const Float4x3U &)=default](struct_luna_1_1_float4x3_u_1ab4c005d814b5418b1a51b07f982fd50a.md)

    Constructs one matrix by coping components from another matrix. 

* [Float4x3U(Float4x3U &&)=default](struct_luna_1_1_float4x3_u_1aaa4b76619d62104bc001e7e932bc5f87.md)

    Assigns one matrix by coping components from another matrix. 

* [Float4x3U & operator=(const Float4x3U &)=default](struct_luna_1_1_float4x3_u_1af95283a18f39cd27f0190e0259e5ef26.md)

    Constructs one matrix by coping components from another matrix. 

* [Float4x3U & operator=(Float4x3U &&)=default](struct_luna_1_1_float4x3_u_1a982f50823614dfde200b48e146b8f56f.md)

    Assigns one matrix by coping components from another matrix. 

* [Float4x3U(const Float4x4 &rhs)](struct_luna_1_1_float4x3_u_1adc9bb618366b6825b3e3963e1fa41cca.md)

    Constructs one matrix by coping components from a [Float4x4](struct_luna_1_1_float4x4.md) matrix. 

* [Float4x3U & operator=(const Float4x4 &rhs)](struct_luna_1_1_float4x3_u_1a4216cf547b7870b3280e1ea4b461dc61.md)

    Assigns one matrix by coping components from a [Float4x4](struct_luna_1_1_float4x4.md) matrix. 

* [Float4x4 to_float4x4(const Float4 &column4=Float4(0.0f, 0.0f, 0.0f, 1.0f)) const](struct_luna_1_1_float4x3_u_1a46d7b2a758e2ece7ec28fa78da523d6c.md)

    Constructs one [Float4x4](struct_luna_1_1_float4x4.md) matrix from this matrix. 

