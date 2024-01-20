# Luna::Simd::permute2_f4

```c++
template <u32, u32, u32, u32>
float4 permute2_f4(float4 a, float4 b)
```

Shuffles single-precision (32-bit) floating-point elements in `a` and `b` based on the control parameter `_SelectX`, `_SelectY`, `_SelectZ` and `_SelectW`, and stores the results in `dst`. 


```
DEFINE SELECT8(a, b, control)
    CASE(control) OF
    0:  res := a.x
    1:  res := a.y
    2:  res := a.z
    3:  res := a.w
    4:  res := b.x
    5:  res := b.y
    6:  res := b.z
    7:  res := b.w
    ESAC
    RETURN res
ENDDEF
dst.x := SELECT4(a, b _SelectX)
dst.y := SELECT4(a, b, _SelectY)
dst.z := SELECT4(a, b, _SelectZ)
dst.w := SELECT4(a, b, _SelectW)
```


