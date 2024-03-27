# Luna::AHI::DeviceDesc
Describes one audio device. 

```c++
struct Luna::AHI::DeviceDesc
```

## Member objects
* [DeviceIODesc playback](struct_luna_1_1_a_h_i_1_1_device_desc_1acedb84b2fd6c8a17c19c2f3de392f909.md)

    Describes the playback stream properties. This will be ignored if audio playback is disabled on this device ( [DeviceFlag::playback](group___a_h_i_1ggad433bdae7e4fec2efb966cfe584aa7fbab97e6a2fbeffb69f3ca5c81325164f3f.md) is not set in `flags`). 

* [DeviceIODesc capture](struct_luna_1_1_a_h_i_1_1_device_desc_1aa3cf3a612a15597cba34a7f0e9873f5d.md)

    Describes the capture stream properties. This will be ignored if audio capture is disabled on this device ( [DeviceFlag::capture](group___a_h_i_1ggad433bdae7e4fec2efb966cfe584aa7fbad7ba9bbfda42b9657f14ee37ef76150b.md) is not set in `flags`). 

* [u32 sample_rate](struct_luna_1_1_a_h_i_1_1_device_desc_1abc7e1bd012e3e4b0f30065588c098af2.md)

    The sample rate of the playback and capture stream. 

* [DeviceFlag flags](struct_luna_1_1_a_h_i_1_1_device_desc_1a286892bec3e22148e39d66f6fd8a82fe.md)

    Additional device flags, like whether to enable playback/capture stream. 

