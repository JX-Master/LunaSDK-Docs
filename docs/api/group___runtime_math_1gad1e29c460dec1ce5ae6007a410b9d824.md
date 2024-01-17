# Luna::lerp

```c++
template <typename _VTy, typename _TTy>
_VTy lerp(_VTy f1, _VTy f2, _TTy t)
```

Performs linear interpolation on the given values. 



## Parameters
* **_VTy**

    The type of the interpolated value. 

* **_TTy**

    The type of the weight value. 

## Parameters
* *in* **f1**

    The first value to interpolate. 

* *in* **f2**

    The second value to interpolate. 

* *in* **t**

    The interpolation weight to use. 

## Return value
Returns the interpolated value. The value is calculated as `f1 * (1 - t) + f2 * t`. 

