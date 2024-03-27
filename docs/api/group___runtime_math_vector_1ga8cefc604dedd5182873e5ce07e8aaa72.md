# Luna::operator-

```c++
Float4 operator-(const Float4 &v1, const Float4 &v2)
```

Subtracts two vectors. 

This function performs the following operations: 
```
[Float4](struct_luna_1_1_float4.md) r;
r.x = v1.x - v2.x;
r.y = v1.y - v2.y;
r.z = v1.z - v2.z;
r.w = v1.w - v2.w;
return r;
```


## Parameters
* *in* **v1**

    The first vector. 

* *in* **v2**

    The second vector. 

## Return value
Returns the result vector. 

