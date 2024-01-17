# Luna::cross

```c++
Float2 cross(const Float2 &v1, const Float2 &v2)
```

Computes the cross product of two vectors. 

This function performs the following operations: 
```
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) [cross](group___runtime_math_vector_1ga9db4baa479fdce3dd851a63db2a5bcfb.md) = v1.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) * v2.y - v1.y * v2.x;
[Float2](struct_luna_1_1_float2.md) result;
result.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) = [cross](group___runtime_math_vector_1ga9db4baa479fdce3dd851a63db2a5bcfb.md);
result.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) = [cross](group___runtime_math_vector_1ga9db4baa479fdce3dd851a63db2a5bcfb.md);
return result;
```


## Parameters
* *in* **v1**

    The first vector. 

* *in* **v2**

    The second vector. 

## Return value
Returns the cross product of two vectors. 

