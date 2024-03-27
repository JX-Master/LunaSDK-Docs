# Luna::operator+

```c++
Float2 operator+(const Float2 &v, f32 s)
```

Adds one vector with one scalar. 

This function performs the following operations: 
```
[Float2](struct_luna_1_1_float2.md) r;
r.x = v.x + s;
r.y = v.y + s;
return r;
```


## Parameters
* *in* **v**

    The vector. 

* *in* **s**

    The scalar. 

## Return value
Returns the result vector. 

