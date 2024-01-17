# Luna::reflect

```c++
Float2 reflect(const Float2 &ivec, const Float2 &nvec)
```

Computes the reflected vector of the input vector. 

This function performs the following operations: 
```
return ivec - (2 * [dot](group___runtime_math_vector_1ga59253c111957a8ea29144ec873bcdc1c.md)(ivec, nvec) * nvec);
```


## Parameters
* *in* **ivec**

    The direction of the incident ray. 

* *in* **nvec**

    The direction of the surface normal. 

## Return value
Returns the direction of the reflected ray. The length of the reflected vector is the same as the length of the `ivec`. 

## Valid Usage
* `nvec` must be a normalized vector. 

