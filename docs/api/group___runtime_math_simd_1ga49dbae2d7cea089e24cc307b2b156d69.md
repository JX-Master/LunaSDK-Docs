# Luna::Simd::permute_f4

```c++
template <u32, u32, u32, u32>
float4 permute_f4(float4 a)
```

Shuffles single-precision (32-bit) floating-point elements in `a` based on the control parameter `_SelectX`, `_SelectY`, `_SelectZ` and `_SelectW`, and stores the results in `dst`. 


```
DEFINE SELECT4(src, control)
    CASE(control) OF
    0:  res := src.x
    1:  res := src.y
    2:  res := src.z
    3:  res := src.w
    ESAC
    RETURN res
ENDDEF
dst.x := SELECT4(a, _SelectX)
dst.y := SELECT4(a, _SelectY)
dst.z := SELECT4(a, _SelectZ)
dst.w := SELECT4(a, _SelectW)
```


