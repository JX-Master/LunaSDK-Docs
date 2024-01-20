# Luna::Color::negate

```c++
Float4 negate(const Float4 &color)
```

Inverts a color value. 

The color is inverted as follows: 
```
[Float4](struct_luna_1_1_float4.md) ret = 1.0f - color;
ret.[w](struct_luna_1_1_float4_1adb390a9d0e1ce3b726f016e547104e35.md) = color.w;
return ret;
```


## Parameters
* *in* **color**

    The color to invert. 

## Return value
Returns the inverted color. 

