# Luna::Quaternion::lerp

```c++
Float4 lerp(const Float4 &q1, const Float4 &q2, f32 t)
```

Performs linear interpolation between two quaternions. 



## Parameters
* *in* **q1**

    The first quaternion. 

* *in* **q2**

    The second quaternion. 

* *in* **t**

    The interpolation weight. `0` to choose `q1`, `1` to choose `q2`. 

## Return value
Returns the result quaternion. 

