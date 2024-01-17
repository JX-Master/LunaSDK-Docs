# Luna::mul

```c++
Float4 mul(const Float4 &vec, const Float4x4 &mat)
```

Performs matrix multiplication between one vector and one matrix. 

This function performs the following operations: 
```
return [Float4](struct_luna_1_1_float4.md)(
    vec.x * mat.r[0].x + vec.y * mat.r[1].x + vec.z * mat.r[2].x + vec.w * mat.r[3].x,
    vec.x * mat.r[0].y + vec.y * mat.r[1].y + vec.z * mat.r[2].y + vec.w * mat.r[3].y,
    vec.x * mat.r[0].z + vec.y * mat.r[1].z + vec.z * mat.r[2].z + vec.w * mat.r[3].z,
    vec.x * mat.r[0].w + vec.y * mat.r[1].w + vec.z * mat.r[2].w + vec.w * mat.r[3].w);
```


## Parameters
* *in* **vec**

    The vector. 

* *in* **mat**

    The matrix. 

## Return value
Returns the result vector. 

