# Luna::Float3x2U
Unaligned 3x2 matrix with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 

```c++
struct Luna::Float3x2U
```

This can be used to store 3x3 affine matrices since the third column is always (0, 0, 1), which can be removed to reduce memory size. 

## Member objects
* [Float2U r[3]](struct_luna_1_1_float3x2_u_1afa9b5055d08f951dc6adc0ee12b30bba.md)

    The array of rows of the matrix. 

## Member functions
* [Float3x2U()=default](struct_luna_1_1_float3x2_u_1a927166d43fdc084226280266d44bfc61.md)

    Constructs one matrix with components uninitialized. 

* [Float3x2U(const Float3x2U &)=default](struct_luna_1_1_float3x2_u_1a7a92d6679339268f2feaf10a5c01c393.md)

    Constructs one matrix by coping components from another matrix. 

* [Float3x2U(Float3x2U &&)=default](struct_luna_1_1_float3x2_u_1ae43f4bd7c2641cdeab0647da1ddbd504.md)

    Assigns one matrix by coping components from another matrix. 

* [Float3x2U & operator=(const Float3x2U &)=default](struct_luna_1_1_float3x2_u_1aa0fd2a269b7158c567085e28f6dac6e9.md)

    Constructs one matrix by coping components from another matrix. 

* [Float3x2U & operator=(Float3x2U &&)=default](struct_luna_1_1_float3x2_u_1a5a2a86866c799dc41321aa1441921652.md)

    Assigns one matrix by coping components from another matrix. 

* [Float3x2U(const Float3x3 &rhs)](struct_luna_1_1_float3x2_u_1a3e54d9efe9dae39d0e6e26626d1314b4.md)

    Constructs one matrix by coping components from a [Float3x3](struct_luna_1_1_float3x3.md) matrix. 

* [Float3x2U & operator=(const Float3x3 &rhs)](struct_luna_1_1_float3x2_u_1ae20517c07138d0d67cecb2eedc06d622.md)

    Assigns one matrix by coping components from a [Float3x3](struct_luna_1_1_float3x3.md) matrix. 

* [Float3x3 to_float3x3(const Float3 &column3=Float3(0.0f, 0.0f, 1.0f)) const](struct_luna_1_1_float3x2_u_1a7fae91e08fd0c469811c779988213d31.md)

    Constructs one [Float3x3](struct_luna_1_1_float3x3.md) matrix from this matrix. 

