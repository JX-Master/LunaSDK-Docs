# Luna::AHI::DeviceIODesc
Describes properties of the playback or capture audio data stream of one device. 

```c++
struct Luna::AHI::DeviceIODesc
```

## Member objects
* [IAdapter* adapter](struct_luna_1_1_a_h_i_1_1_device_i_o_desc_1a1699029b964407120f18c3e57d84be60.md)

    The adapter bound to this stream. This adapter will be used to playback audio data from this stream, or capture audio data and write to this stream. If this is `nullptr`, the primary playback or capture device will be used. 

* [u32 num_channels](struct_luna_1_1_a_h_i_1_1_device_i_o_desc_1aa7ab6da6b807d0d2d3d18a545a3e490a.md)

    The number of channels for one audio frame. 

* [BitDepth bit_depth](struct_luna_1_1_a_h_i_1_1_device_i_o_desc_1a5dee8fe382ed235691acd9246f704222.md)

    The bit depth of one audio sample in this stream. 

