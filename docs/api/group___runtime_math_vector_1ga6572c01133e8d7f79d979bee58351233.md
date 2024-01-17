# Luna::operator-

```c++
Float2 operator-(f32 s, const Float2 &v1)
```

Subtracts one scalar with one vector. 

This function performs the following operations: 
```
[Float2](struct_luna_1_1_float2.md) r;
r.[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) = s - v.x;
r.[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) = s - v.y;
return r;
```


## Parameters
* *in* **s**

    The scalar. 

* *in* **v**

    The vector. 

## Return value
Returns the result vector. 

