# Luna::mul

```c++
Float4 mul(const Float4x4 &mat, const Float4 &vec)
```

Performs matrix multiplication between one matrix and one vector. 

This function performs the following operations: 
```
return [Float4](struct_luna_1_1_float4.md)(
    vec.x * mat.r[0].x + vec.y * mat.r[0].y + vec.z * mat.r[0].z + vec.w * mat.r[0].w,
    vec.x * mat.r[1].x + vec.y * mat.r[1].y + vec.z * mat.r[1].z + vec.w * mat.r[1].w,
    vec.x * mat.r[2].x + vec.y * mat.r[2].y + vec.z * mat.r[2].z + vec.w * mat.r[2].w,
    vec.x * mat.r[3].x + vec.y * mat.r[3].y + vec.z * mat.r[3].z + vec.w * mat.r[3].w);
```


## Parameters
* *in* **mat**

    The matrix. 

* *in* **vec**

    The vector. 

## Return value
Returns the result vector. 

