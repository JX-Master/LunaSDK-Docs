# Luna::mul

```c++
Float3 mul(const Float3 &vec, const Float3x3 &mat)
```

Performs matrix multiplication between one vector and one matrix. 

This function performs the following operations: 
```
return [Float3](struct_luna_1_1_float3.md)(
    vec.x * mat.r[0].x + vec.y * mat.r[1].x + vec.z * mat.r[2].x,
    vec.x * mat.r[0].y + vec.y * mat.r[1].y + vec.z * mat.r[2].y,
    vec.x * mat.r[0].z + vec.y * mat.r[1].z + vec.z * mat.r[2].z);
```


## Parameters
* *in* **vec**

    The vector. 

* *in* **mat**

    The matrix. 

## Return value
Returns the result vector. 

