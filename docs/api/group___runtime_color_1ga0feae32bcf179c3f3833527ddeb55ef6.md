# Luna::Color::to_abgr8

```c++
constexpr u32 to_abgr8(const Float4 &color)
```

Converts one [Float4](struct_luna_1_1_float4.md) linear color value to one 32-bit color value. Every color component takes 8 bits, and is arranged in ABGR order (A in least significant 8 bits, [R](struct_luna_1_1_r.md) in most significant 8 bits). 



## Parameters
* *in* **color**

    The color to convert. 

## Return value
Returns the converted color. 

