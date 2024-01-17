# Luna::mul

```c++
Float3 mul(const Float3x3 &mat, const Float3 &vec)
```

Performs matrix multiplication between one matrix and one vector. 

This function performs the following operations: 
```
return [Float3](struct_luna_1_1_float3.md)(
    vec.x * mat.r[0].x + vec.y * mat.r[0].y + vec.z * mat.r[0].z,
    vec.x * mat.r[1].x + vec.y * mat.r[1].y + vec.z * mat.r[1].z,
    vec.x * mat.r[2].x + vec.y * mat.r[2].y + vec.z * mat.r[2].z);
```


## Parameters
* *in* **mat**

    The matrix. 

* *in* **vec**

    The vector. 

## Return value
Returns the result vector. 

