# Luna::normalize

```c++
Float3 normalize(const Float3 &vec)
```

Normalizes the vector so that the length of the vector is 1. 

This function performs the following operations: 
```
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) len = [length](group___runtime_math_vector_1gad5b84a1689bedf4af98f54c84853583a.md)(vec);
if (len > 0)
{
    len = 1.0f / len;
}
Float3 result;
result.x = vec.x * len;
result.y = vec.y * len;
result.z = vec.z * len;
return result;
```


## Parameters
* *in* **vec**

    The vector to normalize. 

## Return value
Returns the normalized vector. 

