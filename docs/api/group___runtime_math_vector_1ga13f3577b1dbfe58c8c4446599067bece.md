# Luna::clamp

```c++
Float4 clamp(const Float4 &vec, const Float4 &vec_min, const Float4 &vec_max)
```

Clamps the vector to the specified range. 

This function performs the following operations: 
```
[Float3](struct_luna_1_1_float3.md) result;
result.[x](struct_luna_1_1_float3_1a6b05cac69c0301ab972c27ce208373be.md) = vec.x    > vec_min.x ? vec.x    : vec_min.x;
result.[x](struct_luna_1_1_float3_1a6b05cac69c0301ab972c27ce208373be.md) = result.[x](struct_luna_1_1_float3_1a6b05cac69c0301ab972c27ce208373be.md) < vec_max.x ? result.[x](struct_luna_1_1_float3_1a6b05cac69c0301ab972c27ce208373be.md) : vec_max.x;
result.[y](struct_luna_1_1_float3_1ab7291adeb8828a0cba3aedf332c2053d.md) = vec.y    > vec_min.y ? vec.y    : vec_min.y;
result.[y](struct_luna_1_1_float3_1ab7291adeb8828a0cba3aedf332c2053d.md) = result.[y](struct_luna_1_1_float3_1ab7291adeb8828a0cba3aedf332c2053d.md) < vec_max.y ? result.[y](struct_luna_1_1_float3_1ab7291adeb8828a0cba3aedf332c2053d.md) : vec_max.y;
result.[z](struct_luna_1_1_float3_1aac280fcf3516d20b5e3dec5fa770ac50.md) = vec.z    > vec_min.z ? vec.z    : vec_min.z;
result.[z](struct_luna_1_1_float3_1aac280fcf3516d20b5e3dec5fa770ac50.md) = result.[z](struct_luna_1_1_float3_1aac280fcf3516d20b5e3dec5fa770ac50.md) < vec_max.z ? result.[z](struct_luna_1_1_float3_1aac280fcf3516d20b5e3dec5fa770ac50.md) : vec_max.z;
result.w = vec.w    > vec_min.w ? vec.w    : vec_min.w;
result.w = result.w < vec_max.w ? result.w : vec_max.w;
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

