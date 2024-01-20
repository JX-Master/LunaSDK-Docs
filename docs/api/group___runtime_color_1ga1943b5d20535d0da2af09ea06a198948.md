# Luna::Color::to_bgra8

```c++
constexpr u32 to_bgra8(const Float4 &color)
```

Converts one [Float4](struct_luna_1_1_float4.md) linear color value to one 32-bit color value. Every color component takes 8 bits, and is arranged in BGRA order (B in least significant 8 bits, A in most significant 8 bits). 



## Parameters
* *in* **color**

    The color to convert. 

## Return value
Returns the converted color. 

