# Luna::Color::adjust_contrast

```c++
Float4 adjust_contrast(const Float4 &color, f32 contrast)
```

Adjusts color contrast. 

The color contrast is adjusted as follows: 
```
[Float4](struct_luna_1_1_float4.md) ret = ((color - 0.5f) * contrast) + 0.5f;
ret.[w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md) = color.w;
return ret;
```


## Parameters
* *in* **color**

    The color to adjust. 

* *in* **contrast**

    The contrast scale. 

## Return value
Returns the adjusted color. 

