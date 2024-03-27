# Luna::operator+

```c++
Float2 operator+(f32 s, const Float2 &v)
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
* *in* **s**

    The scalar. 

* *in* **v**

    The vector. 

## Return value
Returns the result vector. 

