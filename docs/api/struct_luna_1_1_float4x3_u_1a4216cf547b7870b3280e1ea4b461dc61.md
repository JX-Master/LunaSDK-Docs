# Luna::Float4x3U::operator=

```c++
Float4x3U & operator=(const Float4x4 &rhs)
```

Assigns one matrix by coping components from a [Float4x4](struct_luna_1_1_float4x4.md) matrix. 

The fourth column of the source matrix will be discarded in the constructed matrix. 

## Parameters
* *in* **rhs**

    The matrix to copy components from. 

## Return value
Returns `*this`. 

