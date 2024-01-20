# Luna::Simd::select_f4

```c++
template <u32, u32, u32, u32>
float4 select_f4(float4 a, float4 b)
```

Performs a per-component selection between `a` and `b` based on the control parameter `_SelectX`, `_SelectY`, `_SelectZ` and `_SelectW`, and stores the results in `dst`. 


```
DEFINE SELECT2(a, b control)
    CASE(control) OF
    0:  res := a
    1:  res := b
    ESAC
    RETURN res
ENDDEF
dst.x := SELECT2(a.x, b.x, _SelectX)
dst.y := SELECT4(a.y, b.y, _SelectY)
dst.z := SELECT4(a.z, b.z, _SelectZ)
dst.w := SELECT4(a.w, b.w, _SelectW)
```


