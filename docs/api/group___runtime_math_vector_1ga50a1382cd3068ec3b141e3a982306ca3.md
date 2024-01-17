# Luna::max

```c++
Float2 max(const Float2 &v1, const Float2 &v2)
```

Computes the maximum value of two vectors. 

This function performs the following operations: 
```
[Float2](struct_luna_1_1_float2.md) result;
result.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) = v1.x > v2.x ? v1.x : v2.x;
result.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) = v1.y > v2.y ? v1.y : v2.y;
return result;
```


## Parameters
* *in* **v1**

    The first vector. 

* *in* **v2**

    The second vector. 

## Return value
Returns the maximum value of two vectors. 

