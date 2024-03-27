# Luna::operator/

```c++
Float2 operator/(f32 s, const Float2 &v)
```

Divides one scalar with one vector. 

This function performs the following operations: 
```
[Float2](struct_luna_1_1_float2.md) r;
r.x = s / v.x;
r.y = s / v.y;
return r;
```


## Parameters
* *in* **s**

    The scalar. 

* *in* **v**

    The vector. 

## Return value
Returns the result vector. 

