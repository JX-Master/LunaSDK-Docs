# Luna::RHI::TextureViewDesc::array_size

```c++
u32 array_size
```

The number of array elements included in this view. [Array](class_luna_1_1_array.md) elements in range [`array_slice`, `array_slice + array_size`) will be included in this view. 

If this is [U32_MAX](group___runtime_base_type_1ga645ed2bd2baa2b4ed82d67bc5597ef47.md), all array elements beginning from `array_slice` will be included in this view.

This must be `1` if `type` is not an texture array or texture cube type. This must be times of 6 if `type` is a texture cube type. 

