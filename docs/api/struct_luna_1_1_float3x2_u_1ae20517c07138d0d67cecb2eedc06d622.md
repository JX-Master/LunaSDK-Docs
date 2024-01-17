# Luna::Float3x2U::operator=

```c++
Float3x2U & operator=(const Float3x3 &rhs)
```

Assigns one matrix by coping components from a [Float3x3](struct_luna_1_1_float3x3.md) matrix. 

The third column of the source matrix will be discarded in the constructed matrix. 

## Parameters
* *in* **rhs**

    The matrix to copy components from. 

## Return value
Returns `*this`. 

