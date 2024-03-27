# Luna::operator-

```c++
Float4 operator-(f32 s, const Float4 &v)
```

Subtracts one scalar with one vector. 

This function performs the following operations: 
```
[Float4](struct_luna_1_1_float4.md) r;
r.x = s - v.x;
r.y = s - v.y;
r.z = s - v.z;
r.w = s - v.w;
return r;
```


## Parameters
* *in* **s**

    The scalar. 

* *in* **v**

    The vector. 

## Return value
Returns the result vector. 

