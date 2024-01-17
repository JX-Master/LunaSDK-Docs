# Vectors
## Types
* [Luna::Float2](struct_luna_1_1_float2.md)

    2D vector type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 


* [Luna::Vec2U](struct_luna_1_1_vec2_u.md)

    A generalized version of 2D vector. This vector type does not have specific alignment requirement. 


* [Luna::Float3](struct_luna_1_1_float3.md)

    3D vector type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 


* [Luna::Vec3U](struct_luna_1_1_vec3_u.md)

    A generalized version of 3D vector. This vector type does not have specific alignment requirement. 


* [Luna::Float4](struct_luna_1_1_float4.md)

    4D vector type with [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) components. 


* [Luna::Vec4U](struct_luna_1_1_vec4_u.md)

    A generalized version of 4D vector. This vector type does not have specific alignment requirement. 


## Alias types
* [using Float2U =  Vec2U<f32>](group___runtime_math_vector_1gabab54b920d9357aa09bc646f11c3ee39.md)

    Unaligned 2D floating-point vector type. 

* [using Int2U =  Vec2U<i32>](group___runtime_math_vector_1gae0419540c3fd1b44ddfe9fb7e22e66a5.md)

    Unaligned 2D signed integer vector type. 

* [using UInt2U =  Vec2U<u32>](group___runtime_math_vector_1ga4bdc4df878db6ed57f67bf017bd3e054.md)

    Unaligned 2D unsigned integer vector type. 

* [using Float3U =  Vec3U<f32>](group___runtime_math_vector_1ga5fe5956fb6b821b5c288d136834b85e3.md)

    Unaligned 3D floating-point vector type. 

* [using Int3U =  Vec3U<i32>](group___runtime_math_vector_1gaa1ac15cfa41b63141d2503a660b5a12c.md)

    Unaligned 3D signed integer vector type. 

* [using UInt3U =  Vec3U<u32>](group___runtime_math_vector_1gab0fb51d38608d6a92c85b7d68b44b84f.md)

    Unaligned 3D unsigned integer vector type. 

* [using Float4U =  Vec4U<f32>](group___runtime_math_vector_1gae22dfad19c564ddfb75616a3a6d40db2.md)

    Unaligned 4D floating-point vector type. 

* [using Int4U =  Vec4U<i32>](group___runtime_math_vector_1gab2db19518dcdfd3ef71cbd86623288c4.md)

    Unaligned 4D signed integer vector type. 

* [using UInt4U =  Vec4U<u32>](group___runtime_math_vector_1ga9fb64fa3c1b46f9de519fe6ad51e6948.md)

    Unaligned 4D unsigned integer vector type. 

## Functions
* [Float2 operator+(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1ga9a82e76e04f57052d5d9ddf27d64ad5d.md)

    Adds two vectors. 

* [Float2 operator-(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1gaa7a740c2b400ff90572a1755e0f1404a.md)

    Subtracts two vectors. 

* [Float2 operator*(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1ga8f7d95857808873e8f9883007d09c89d.md)

    Multiplies two vectors. 

* [Float2 operator/(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1ga0d08afeda928faaa4dc0be35e57dddff.md)

    Divides two vectors. 

* [Float2 operator+(const Float2 &v, f32 s)](group___runtime_math_vector_1ga526a1c91427b57f4da18a548eeb2b0d3.md)

    Adds one vector with one scalar. 

* [Float2 operator+(f32 s, const Float2 &v)](group___runtime_math_vector_1ga604166e5a89290d128980a32279123e6.md)

    Adds one vector with one scalar. 

* [Float2 operator-(const Float2 &v, f32 s)](group___runtime_math_vector_1ga0d296caacd4e6d37f000db132fcd5826.md)

    Subtracts one vector with one scalar. 

* [Float2 operator-(f32 s, const Float2 &v1)](group___runtime_math_vector_1ga6572c01133e8d7f79d979bee58351233.md)

    Subtracts one scalar with one vector. 

* [Float2 operator*(const Float2 &v, f32 s)](group___runtime_math_vector_1gae8f027626cf2b670917140012d97dd3a.md)

    Multiplies one vector with one scalar. 

* [Float2 operator*(f32 s, const Float2 &v)](group___runtime_math_vector_1gab5e8ed7ed1dd81c129cae1d03d6f6baa.md)

    Multiplies one vector with one scalar. 

* [Float2 operator/(const Float2 &v, f32 s)](group___runtime_math_vector_1ga1f73b7901be57313efc10830c96ca001.md)

    Divides one vector with one scalar. 

* [Float2 operator/(f32 s, const Float2 &v)](group___runtime_math_vector_1gac3a696a4689af445f06adbb579423cd0.md)

    Divides one scalar with one vector. 

* [bool in_bounds(const Float2 &point, const Float2 &min_bound, const Float2 &max_bound)](group___runtime_math_vector_1gacc8077d0ecacdbb491bf39afbb0ef9f5.md)

    Checks whether the point is in the specified boundary. 

* [f32 length(const Float2 &vec)](group___runtime_math_vector_1gad5b84a1689bedf4af98f54c84853583a.md)

    Computes the length of the vector. 

* [f32 length_squared(const Float2 &vec)](group___runtime_math_vector_1gaa58b9014b510c0158a3ba28e5bef7f95.md)

    Computes the squared length of the vector. 

* [f32 dot(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1ga59253c111957a8ea29144ec873bcdc1c.md)

    Computes the dot product of two vectors. 

* [Float2 cross(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1ga9db4baa479fdce3dd851a63db2a5bcfb.md)

    Computes the cross product of two vectors. 

* [Float2 normalize(const Float2 &vec)](group___runtime_math_vector_1gac269f35249b0e08c3bb7e447a582bf0d.md)

    Normalizes the vector so that the length of the vector is 1. 

* [Float2 clamp(const Float2 &vec, const Float2 &vec_min, const Float2 &vec_max)](group___runtime_math_vector_1gaba2e604b8a4120e06f6581b68ba1d754.md)

    Clamps the vector to the specified range. 

* [f32 distance(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1gacf0c770e2335339afd44bf1b8753a4ab.md)

    Computes the distance between two points. 

* [f32 distance_squared(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1gac24d3dd2470a97cecab0f789ec205666.md)

    Computes the squared distance between two points. 

* [Float2 min(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1ga4a2570340193114c8bc9f119f6e68da7.md)

    Computes the minimum value of two vectors. 

* [Float2 max(const Float2 &v1, const Float2 &v2)](group___runtime_math_vector_1ga50a1382cd3068ec3b141e3a982306ca3.md)

    Computes the maximum value of two vectors. 

* [Float2 lerp(const Float2 &v1, const Float2 &v2, f32 t)](group___runtime_math_vector_1ga12b87861df0c704d4c43d4d2090ea0d8.md)

    Performs linear interpolation between two vectors. 

* [Float2 smoothstep(const Float2 &v1, const Float2 &v2, f32 t)](group___runtime_math_vector_1gab0e2361a3cd712476d19f83fb49b4a2a.md)

    Performs smoothstep interpolation between two vectors. 

* [Float2 barycentric(const Float2 &v1, const Float2 &v2, const Float2 &v3, f32 f, f32 g)](group___runtime_math_vector_1ga94256e016105efb6354c48482bc3dcd0.md)

    Performs barycentric interpolation between three vectors. 

* [Float2 catmull_rom(const Float2 &v1, const Float2 &v2, const Float2 &v3, const Float2 &v4, f32 t)](group___runtime_math_vector_1gab20c335ec45c96233919e249d4e2c2dd.md)

    Performs centripetal Catmull–Rom spline interpolation. 

* [Float2 hermite(const Float2 &v1, const Float2 &t1, const Float2 &v2, const Float2 &t2, f32 t)](group___runtime_math_vector_1gadafffd97ab96cb3b0ad07b7652a80f59.md)

    Performs Hermite spline interpolation. 

* [Float2 reflect(const Float2 &ivec, const Float2 &nvec)](group___runtime_math_vector_1gabea76eede07c31ee3680196ac934be7c.md)

    Computes the reflected vector of the input vector. 

* [Float2 refract(const Float2 &ivec, const Float2 &nvec, f32 refraction_index)](group___runtime_math_vector_1gaf7ce2bb5a64b2023e7d6d50fee3dbf2a.md)

    Computes the refracted vector of the input vector. 

* [Float3 operator+(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1gacf33deea93b11123f7061ba59977fa8d.md)

    Adds two vectors. 

* [Float3 operator-(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1gabc81d2be7fa061e4b2691fc54a5956d6.md)

    Subtracts two vectors. 

* [Float3 operator*(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1ga84299fb20f7d907e23017cb9c42b21c4.md)

    Multiplies two vectors. 

* [Float3 operator/(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1ga43553ea39b38b776fd7b1f611f829d0b.md)

    Divides two vectors. 

* [Float3 operator+(const Float3 &v, f32 s)](group___runtime_math_vector_1gaf5d0980db7049f500368c7e2a1260340.md)

    Adds one vector with one scalar. 

* [Float3 operator+(f32 s, const Float3 &v)](group___runtime_math_vector_1ga2b13a0441d1a84ea73703fce3b97ff67.md)

    Adds one vector with one scalar. 

* [Float3 operator-(const Float3 &v, f32 s)](group___runtime_math_vector_1ga686c2a979cae59e8ff5d4dc1e8ecd633.md)

    Subtracts one vector with one scalar. 

* [Float3 operator-(f32 s, const Float3 &v)](group___runtime_math_vector_1gae7915f811b2c87f98c4a3518133a2bc6.md)

    Subtracts one scalar with one vector. 

* [Float3 operator*(const Float3 &v, f32 s)](group___runtime_math_vector_1ga67852948f44a593a5305975ece9aae5e.md)

    Multiplies one vector with one scalar. 

* [Float3 operator*(f32 s, const Float3 &v)](group___runtime_math_vector_1ga223798832041e50b6f9197e6d447b048.md)

    Multiplies one vector with one scalar. 

* [Float3 operator/(const Float3 &v, f32 s)](group___runtime_math_vector_1ga65478f849d656a92f8c1307097e5f171.md)

    Divides one vector with one scalar. 

* [Float3 operator/(f32 s, const Float3 &v)](group___runtime_math_vector_1ga3d9dc28c15adb825d8610999e50efd0b.md)

    Divides one scalar with one vector. 

* [bool in_bounds(const Float3 &point, const Float3 &min_bound, const Float3 &max_bound)](group___runtime_math_vector_1gac07bd41e1aa485ba891ab871bb0e76ec.md)

    Checks whether the point is in the specified boundary. 

* [f32 length(const Float3 &vec)](group___runtime_math_vector_1ga350f81c74f37b897ad37ac0654814b94.md)

    Computes the length of the vector. 

* [f32 length_squared(const Float3 &vec)](group___runtime_math_vector_1ga78ceadd5ae8cada6d5b049a1e0f8a7b3.md)

    Computes the squared length of the vector. 

* [f32 dot(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1ga6302d033a046bcb77fe7bbc2049797e8.md)

    Computes the dot product of two vectors. 

* [Float3 cross(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1ga410490ab09f3272b3826ddb25f8c2584.md)

    Computes the cross product of two vectors. 

* [Float3 normalize(const Float3 &vec)](group___runtime_math_vector_1gafef9d01b95a5c3d6b901bcdb028359c3.md)

    Normalizes the vector so that the length of the vector is 1. 

* [Float3 clamp(const Float3 &vec, const Float3 &vec_min, const Float3 &vec_max)](group___runtime_math_vector_1gac05c1c78a14c6c061a75d9cc3bf70736.md)

    Clamps the vector to the specified range. 

* [f32 distance(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1ga2e02eb26a54ec9a961aa950c2421daf2.md)

    Computes the distance between two points. 

* [f32 distance_squared(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1ga76726e806deaf27ee1e223481a71ab09.md)

    Computes the squared distance between two points. 

* [Float3 min(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1gaffb76914034a946c841a77bae9a36147.md)

    Computes the minimum value of two vectors. 

* [Float3 max(const Float3 &v1, const Float3 &v2)](group___runtime_math_vector_1gaf0ca16e96ef11fba7b7423a5564ff0ea.md)

    Computes the maximum value of two vectors. 

* [Float3 lerp(const Float3 &v1, const Float3 &v2, f32 t)](group___runtime_math_vector_1ga1de22e999e75616aaef28a6451fbea76.md)

    Performs linear interpolation between two vectors. 

* [Float3 smoothstep(const Float3 &v1, const Float3 &v2, f32 t)](group___runtime_math_vector_1ga931ce1d30b1137121d9623c50d9555e0.md)

    Performs smoothstep interpolation between two vectors. 

* [Float3 barycentric(const Float3 &v1, const Float3 &v2, const Float3 &vec3, f32 f, f32 g)](group___runtime_math_vector_1ga90a764af4cf1ad7608e0e9ac1ccb9d87.md)

    Performs barycentric interpolation between three vectors. 

* [Float3 catmull_rom(const Float3 &v1, const Float3 &v2, const Float3 &vec3, const Float3 &vec4, f32 t)](group___runtime_math_vector_1ga4f8917d508734c1908b646c6cf7fa71d.md)

    Performs centripetal Catmull–Rom spline interpolation. 

* [Float3 hermite(const Float3 &v1, const Float3 &t1, const Float3 &v2, const Float3 &t2, f32 t)](group___runtime_math_vector_1ga183fbc9d30e3447894e3ae3e980cceba.md)

    Performs Hermite spline interpolation. 

* [Float3 reflect(const Float3 &ivec, const Float3 &nvec)](group___runtime_math_vector_1ga7208b6459e08f7c032d66cf4e4e46a51.md)

    Computes the reflected vector of the input vector. 

* [Float3 refract(const Float3 &ivec, const Float3 &nvec, f32 refraction_index)](group___runtime_math_vector_1ga81e6491c0a2d7e653ab546b689fc4b40.md)

    Computes the refracted vector of the input vector. 

* [Float4 operator+(const Float4 &v1, const Float4 &v2)](group___runtime_math_vector_1ga21305ac283447e58c80c03665cb6103b.md)

    Adds two vectors. 

* [Float4 operator-(const Float4 &v1, const Float4 &v2)](group___runtime_math_vector_1ga8cefc604dedd5182873e5ce07e8aaa72.md)

    Subtracts two vectors. 

* [Float4 operator*(const Float4 &v1, const Float4 &v2)](group___runtime_math_vector_1ga100920117430ed0732c77c527d3127f9.md)

    Multiplies two vectors. 

* [Float4 operator/(const Float4 &v1, const Float4 &v2)](group___runtime_math_vector_1gabf27b3916d94029a810ee9c41ab2a8bd.md)

    Divides two vectors. 

* [Float4 operator+(const Float4 &v, f32 s)](group___runtime_math_vector_1ga8e9636151c0fb25fa6def7054a4bf1f8.md)

    Adds one vector with one scalar. 

* [Float4 operator+(f32 s, const Float4 &v)](group___runtime_math_vector_1ga7ace60ddc2427079159a4ffaf316875c.md)

    Adds one vector with one scalar. 

* [Float4 operator-(const Float4 &v, f32 s)](group___runtime_math_vector_1ga34293ef5b5b23c11d94e24a2047a6aa8.md)

    Subtracts one vector with one scalar. 

* [Float4 operator-(f32 s, const Float4 &v)](group___runtime_math_vector_1ga4d68c2b88e9c63de2dcd184a967b76a7.md)

    Subtracts one scalar with one vector. 

* [Float4 operator*(const Float4 &v, f32 s)](group___runtime_math_vector_1ga14ab591b36b4774107ee3dc9068f25d3.md)

    Multiplies one vector with one scalar. 

* [Float4 operator*(f32 s, const Float4 &v)](group___runtime_math_vector_1ga09d30b86a7c779c6a55aeb21caccfec0.md)

    Multiplies one vector with one scalar. 

* [Float4 operator/(const Float4 &v, f32 s)](group___runtime_math_vector_1ga344a7b70af08db7ceda682e1e5a71bfd.md)

    Divides one vector with one scalar. 

* [Float4 operator/(f32 s, const Float4 &v)](group___runtime_math_vector_1ga1b8a46bf13e4e513d1f66e8f781af1c2.md)

    Divides one scalar with one vector. 

* [bool in_bounds(const Float4 &point, const Float4 &min_bound, const Float4 &max_bound)](group___runtime_math_vector_1ga202821a343feff651a6966de2856d41c.md)

    Checks whether the point is in the specified boundary. 

* [f32 length(const Float4 &vec)](group___runtime_math_vector_1gae099b809dec4ea0fab6db54e04f82ebc.md)

    Computes the length of the vector. 

* [f32 length_squared(const Float4 &vec)](group___runtime_math_vector_1gaed79457a78f656167a11ac4baee9a071.md)

    Computes the squared length of the vector. 

* [f32 dot(const Float4 &v1, const Float4 &v2)](group___runtime_math_vector_1ga4eafe3f525faff411187a6b36a206cf0.md)

    Computes the dot product of two vectors. 

* [Float4 cross(const Float4 &v1, const Float4 &v2, const Float4 &v3)](group___runtime_math_vector_1gad1c8ac36904c8b2cc3d3e4fd94c8b743.md)

    Computes the cross product of two vectors. 

* [Float4 normalize(const Float4 &vec)](group___runtime_math_vector_1ga77ed8221460bb15d77ad778f793323cb.md)

    Normalizes the vector so that the length of the vector is 1. 

* [Float4 clamp(const Float4 &vec, const Float4 &vec_min, const Float4 &vec_max)](group___runtime_math_vector_1ga13f3577b1dbfe58c8c4446599067bece.md)

    Clamps the vector to the specified range. 

* [f32 distance(const Float4 &v1, const Float4 &v2)](group___runtime_math_vector_1ga369da5cd1c862e96d54b7a9088db3959.md)

    Computes the distance between two points. 

* [f32 distance_squared(const Float4 &v1, const Float4 &v2)](group___runtime_math_vector_1ga29d6849a6d833dd8b5877c72bc86559e.md)

    Computes the squared distance between two points. 

* [Float4 min(const Float4 &v1, const Float4 &v2)](group___runtime_math_vector_1ga6e259fbd6f057c1c54498fa29c0c8c57.md)

    Computes the minimum value of two vectors. 

* [Float4 max(const Float4 &v1, const Float4 &v2)](group___runtime_math_vector_1ga716102a28b7565436b68a4b13f20092e.md)

    Computes the maximum value of two vectors. 

* [Float4 lerp(const Float4 &v1, const Float4 &v2, f32 t)](group___runtime_math_vector_1ga3034351ba07a7b4d72ff40e5a1314687.md)

    Performs linear interpolation between two vectors. 

* [Float4 smoothstep(const Float4 &v1, const Float4 &v2, f32 t)](group___runtime_math_vector_1ga601750f061466e2d88a42a91b57ee330.md)

    Performs smoothstep interpolation between two vectors. 

* [Float4 barycentric(const Float4 &v1, const Float4 &v2, const Float4 &vec3, f32 f, f32 g)](group___runtime_math_vector_1ga7bac17ffc21df02c03a7ecd8363c5273.md)

    Performs barycentric interpolation between three vectors. 

* [Float4 catmull_rom(const Float4 &v1, const Float4 &v2, const Float4 &vec3, const Float4 &vec4, f32 t)](group___runtime_math_vector_1ga333e16158b92ece49303bcd8e18453eb.md)

    Performs centripetal Catmull–Rom spline interpolation. 

* [Float4 hermite(const Float4 &v1, const Float4 &t1, const Float4 &v2, const Float4 &t2, f32 t)](group___runtime_math_vector_1ga004d4e7ba8ae168bd4d644a5b0667217.md)

    Performs Hermite spline interpolation. 

* [Float4 reflect(const Float4 &ivec, const Float4 &nvec)](group___runtime_math_vector_1ga39c368ec63e6d024432eb80c4eccd02b.md)

    Computes the reflected vector of the input vector. 

* [Float4 refract(const Float4 &ivec, const Float4 &nvec, f32 refraction_index)](group___runtime_math_vector_1ga14911a6855046301c6c66e90903b622d.md)

    Computes the refracted vector of the input vector. 

* [typeinfo_t float2_type()](group___runtime_math_vector_1ga1326f0b9412ee98c05667668663c71c3.md)

    Gets the type object of [Float2](struct_luna_1_1_float2.md). 

* [typeinfo_t float3_type()](group___runtime_math_vector_1ga5b4aba7139ba9a7516f1c966c7c75271.md)

    Gets the type object of [Float3](struct_luna_1_1_float3.md). 

* [typeinfo_t float4_type()](group___runtime_math_vector_1gae350f81b0bbf848520a97948f90af6fc.md)

    Gets the type object of [Float4](struct_luna_1_1_float4.md). 

* [typeinfo_t vec2u_type()](group___runtime_math_vector_1ga3c2b76b2ca4aca8e5686a106b06199e2.md)

    Gets the type object of [Vec2U](struct_luna_1_1_vec2_u.md). The type object is a generic structure type that should be instanced before use. 

* [typeinfo_t vec3u_type()](group___runtime_math_vector_1ga72fd303366a6edb10010ab7410a42efb.md)

    Gets the type object of [Vec3U](struct_luna_1_1_vec3_u.md). The type object is a generic structure type that should be instanced before use. 

* [typeinfo_t vec4u_type()](group___runtime_math_vector_1gafd22c9beaa449c7dbb6f29623cdcdf27.md)

    Gets the type object of [Vec4U](struct_luna_1_1_vec4_u.md). The type object is a generic structure type that should be instanced before use. 

