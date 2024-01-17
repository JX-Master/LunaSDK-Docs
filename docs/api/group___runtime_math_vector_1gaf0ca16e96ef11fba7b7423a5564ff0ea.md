# Luna::max

```c++
Float3 max(const Float3 &v1, const Float3 &v2)
```

Computes the maximum value of two vectors. 

This function performs the following operations: 
```
[Float3](struct_luna_1_1_float3.md) result;
result.[x](struct_luna_1_1_float3_1a6b05cac69c0301ab972c27ce208373be.md) = v1.x > v2.x ? v1.x : v2.x;
result.[y](struct_luna_1_1_float3_1ab7291adeb8828a0cba3aedf332c2053d.md) = v1.y > v2.y ? v1.y : v2.y;
result.[z](struct_luna_1_1_float3_1aac280fcf3516d20b5e3dec5fa770ac50.md) = v1.z > v2.z ? v1.z : v2.z;
return result;
```


## Parameters
* *in* **v1**

    The first vector. 

* *in* **v2**

    The second vector. 

## Return value
Returns the maximum value of two vectors. 

