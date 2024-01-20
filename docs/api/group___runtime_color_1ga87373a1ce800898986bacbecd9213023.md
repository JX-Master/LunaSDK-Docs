# Luna::Color::adjust_saturation

```c++
Float4 adjust_saturation(const Float4 &color, f32 sat)
```

Adjusts color saturation. 

The color saturation is adjusted as follows: 
```
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) lum = [dot](group___runtime_math_vector_1ga59253c111957a8ea29144ec873bcdc1c.md)(color, [Float4](struct_luna_1_1_float4.md)(0.2125f, 0.7154f, 0.0721f, 0.0f));
[Float4](struct_luna_1_1_float4.md) ret = (color - lum) * sat + lum;
ret.[w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md) = color.w;
return ret;
```


## Parameters
* *in* **color**

    The color to adjust. 

* *in* **sat**

    The saturation scale. 

## Return value
Returns the adjusted color. 

