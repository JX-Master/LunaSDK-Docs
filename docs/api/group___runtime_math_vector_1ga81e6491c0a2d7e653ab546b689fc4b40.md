# Luna::refract

```c++
Float3 refract(const Float3 &ivec, const Float3 &nvec, f32 refraction_index)
```

Computes the refracted vector of the input vector. 

This function performs the following operations: 
```
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) proj = [dot](group___runtime_math_vector_1ga59253c111957a8ea29144ec873bcdc1c.md)(ivec, nvec);
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) deter = 1.0f - refraction_index * refraction_index * (1.0f - proj * proj);
if (deter >= 0.0f)
{
    return ivec * refraction_index - nvec * (refraction_index * proj + sqrtf(deter));
}
return Float3(0.0f);
```


## Parameters
* *in* **ivec**

    The direction of the incident ray. 

* *in* **nvec**

    The direction of the surface normal. 

* *in* **refraction_index**

    The refraction index. 

## Return value
Returns the direction of the refracted ray. The length of the refracted ray is normalized. Returns {0, 0} if the incident angle of `ivec` is too big that no refraction can occur (full reflection). 

## Valid Usage
* Both `ivec` and `nvec` must be normalized vectors.

* `refraction_index` must be a value greater than `0`. 

