# Luna::operator-

```c++
Float3 operator-(f32 s, const Float3 &v)
```

Subtracts one scalar with one vector. 

This function performs the following operations: 
```
[Float3](struct_luna_1_1_float3.md) r;
r.[x](struct_luna_1_1_float3_1a6b05cac69c0301ab972c27ce208373be.md) = s - v.x;
r.[y](struct_luna_1_1_float3_1ab7291adeb8828a0cba3aedf332c2053d.md) = s - v.y;
r.[z](struct_luna_1_1_float3_1aac280fcf3516d20b5e3dec5fa770ac50.md) = s - v.z;
return r;
```


## Parameters
* *in* **s**

    The scalar. 

* *in* **v**

    The vector. 

## Return value
Returns the result vector. 

