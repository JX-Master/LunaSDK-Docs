# Luna::clamp

```c++
template <typename _Ty1, typename _Ty2, typename _Ty3>
_Ty1 clamp(_Ty1 v, _Ty2 min_v, _Ty3 max_v)
```

Clamps the value to the specified range. 



## Parameters
* **_Ty1**

    The type of the value to clamp. 

* **_Ty2**

    The type of the low clamp threshold. 

* **_Ty3**

    The type of the high clamp threshold. 

## Parameters
* *in* **v**

    The value to clamp. 

* *in* **min_v**

    The low clamp threshold. 

* *in* **max_v**

    The high clamp threshold. 

## Return value
Returns the value clamped to [`min_v`, `max_v`]. 

