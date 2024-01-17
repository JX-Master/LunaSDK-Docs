# Luna::Float2::operator+=

```c++
Float2 & operator+=(const Float2 &v)
```

Adds this vector with one vector, and stores the result to this vector. 

This function performs the following operations: 
```
this->[x](struct_luna_1_1_float2_1a6b05cac69c0301ab972c27ce208373be.md) += v.x;
this->[y](struct_luna_1_1_float2_1ab7291adeb8828a0cba3aedf332c2053d.md) += v.y;
```


## Parameters
* *in* **v**

    The vector to add. 

## Return value
Returns `*this`. 

