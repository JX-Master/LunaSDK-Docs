# Luna::operator/

```c++
Float3 operator/(f32 s, const Float3 &v)
```

Divides one scalar with one vector. 

This function performs the following operations: 
```
[Float3](struct_luna_1_1_float3.md) r;
r.x = s / v.x;
r.y = s / v.y;
r.z = s / v.z;
return r;
```


## Parameters
* *in* **s**

    The scalar. 

* *in* **v**

    The vector. 

## Return value
Returns the result vector. 

