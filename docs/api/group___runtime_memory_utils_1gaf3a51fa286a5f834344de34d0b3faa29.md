# Luna::align_upper

```c++
template <typename _Ty1, typename _Ty2>
constexpr _Ty1 align_upper(_Ty1 origin, _Ty2 alignment)
```

Returns the address/size that aligns the origin address/size to the nearest matched aligned address/size that is greater than or equal to the the origin address/size. 



## Parameters
* *in* **origin**

    The unaligned address/size. 

* *in* **alignment**

    The alignment boundary. If alignment is 0, `origin` will be returned as-is. 

## Return value
Returns the aligned address/size. 

