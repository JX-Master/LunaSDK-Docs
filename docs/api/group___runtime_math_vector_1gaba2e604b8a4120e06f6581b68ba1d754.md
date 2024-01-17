# Luna::clamp

```c++
Float2 clamp(const Float2 &vec, const Float2 &vec_min, const Float2 &vec_max)
```

Clamps the vector to the specified range. 

This function performs the following operations: 
```
[Float2](struct_luna_1_1_float2.md) result;
result.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) = vec.x    > vec_min.x ? vec.x    : vec_min.x;
result.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) = result.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) < vec_max.x ? result.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) : vec_max.x;
result.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) = vec.y    > vec_min.y ? vec.y    : vec_min.y;
result.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) = result.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) < vec_max.y ? result.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) : vec_max.y;
return result;
```


## Parameters
* *in* **vec**

    The vector to clamp. 

* *in* **vec_min**

    The lower clamp value. 

* *in* **vec_max**

    The upper clamp value. 

## Return value
Returns the clampd vector. 

