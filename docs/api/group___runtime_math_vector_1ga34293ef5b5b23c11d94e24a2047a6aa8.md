# Luna::operator-

```c++
Float4 operator-(const Float4 &v, f32 s)
```

Subtracts one vector with one scalar. 

This function performs the following operations: 
```
[Float4](struct_luna_1_1_float4.md) r;
r.x = v.x - s;
r.y = v.y - s;
r.z = v.z - s;
r.w = v.w - s;
return r;
```


## Parameters
* *in* **v**

    The vector. 

* *in* **s**

    The scalar. 

## Return value
Returns the result vector. 

