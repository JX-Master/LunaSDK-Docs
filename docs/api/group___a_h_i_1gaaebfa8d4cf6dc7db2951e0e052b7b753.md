# Luna::AHI::BitDepth

```c++
enum BitDepth : u8
{
    unspecified= 0
    u8= 1
    s16= 2
    s24= 3
}
```

Specifies bit depth of audio samples. 

## Options
* [unspecified](group___a_h_i_1ggaaebfa8d4cf6dc7db2951e0e052b7b753ad415f0e30c471dfdd9bc4f827329ef48.md)

    Use system-preferred bit depth. This can only be used when creating audio devices. 

* [u8](group___a_h_i_1ggaaebfa8d4cf6dc7db2951e0e052b7b753a077393852be20e37026d6281827662f2.md)

    8-bit unsigned integer ranged in [0, 255]. 

* [s16](group___a_h_i_1ggaaebfa8d4cf6dc7db2951e0e052b7b753a396f387f2e22fb295b941df41a05f0dc.md)

    16-bit signed integer ranged in [-32768, 32767]. 

* [s24](group___a_h_i_1ggaaebfa8d4cf6dc7db2951e0e052b7b753a08eca8f85ffc96a4ce12615a61969e9d.md)

    24-bit signed integer ranged in [-8388608, 8388607]. 

