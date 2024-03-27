# Luna::RHI::TextureAddressMode

```c++
enum TextureAddressMode : u8
{
    repeat
    mirror
    clamp
    border
}
```

Specifies the texture address mode for samplers when the sample position does not fall in range [0, 1]. 

## Options
* [repeat](group___r_h_i_1ggaf6eef5ace6d21fcf0d846e6950ed179da32cf6da134a8b268cf4ab6b79a9a5ad9.md)

    Given the input position `x`, the sample position is computed as `x - floor(x)`. 

* [mirror](group___r_h_i_1ggaf6eef5ace6d21fcf0d846e6950ed179dafbe322a89bc0ba531c3f0050e3935f28.md)

    Given the input position `x`, the sample position is computed as `1 - abs(mod(x, 2) - 1)`

* [clamp](group___r_h_i_1ggaf6eef5ace6d21fcf0d846e6950ed179daa597a055c00d084069e4bb23dc789ac9.md)

    Given the input position `x`, the sample position is computed as `clamp(x, 0, 1)`. 

* [border](group___r_h_i_1ggaf6eef5ace6d21fcf0d846e6950ed179da2de42fbb00305f8282310f1b3e10ce9a.md)

    Outputs one constant color if input position x is not in range [0, 1]. 

