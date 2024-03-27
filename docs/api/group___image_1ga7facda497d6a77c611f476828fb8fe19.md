# Luna::Image::ImageFormat

```c++
enum ImageFormat : u8
{
    unknown
    r8_unorm
    rg8_unorm
    rgb8_unorm
    rgba8_unorm
    r16_unorm
    rg16_unorm
    rgb16_unorm
    rgba16_unorm
    r32_float
    rg32_float
    rgb32_float
    rgba32_float
}
```

Formats that can be saved in one image file (except DDS, which is identified by [DDSFormat](group___image_1gaadf6475eb5b53a62dfbde2a85e07bc25.md)). 

## Options
* [unknown](group___image_1gga7facda497d6a77c611f476828fb8fe19aad921d60486366258809553a3db49a4a.md)

    The image format is unknown. 

* [r8_unorm](group___image_1gga7facda497d6a77c611f476828fb8fe19a18cb52b2cae3cdc3c65dea6ee91f0944.md)

    Format with one component of 8-bit normalized unsigned integer. Supported by all formats except .hdr. 

* [rg8_unorm](group___image_1gga7facda497d6a77c611f476828fb8fe19a50b96dac1c585e3f58ca90b52016fd75.md)

    Format with two components of 8-bit normalized unsigned integer. Supported by all formats except .hdr. 

* [rgb8_unorm](group___image_1gga7facda497d6a77c611f476828fb8fe19a5f8229d8ffdaf12da8cbda05757fbd94.md)

    Format with three components of 8-bit normalized unsigned integer. Supported by all formats except .hdr. 

* [rgba8_unorm](group___image_1gga7facda497d6a77c611f476828fb8fe19a9c30a57b56cc2f3d801bdba7abba4407.md)

    Format with four components of 8-bit normalized unsigned integer. Supported by all formats except .hdr. 

* [r16_unorm](group___image_1gga7facda497d6a77c611f476828fb8fe19a4a4bab63c1551583499c38efd95b3c5c.md)

    Format with one component of 16-bit normalized unsigned integer. Supported only by .png. 

* [rg16_unorm](group___image_1gga7facda497d6a77c611f476828fb8fe19a3c7f7567b374922870b17fdc546b20b8.md)

    Format with two components of 16-bit normalized unsigned integer. Supported only by .png. 

* [rgb16_unorm](group___image_1gga7facda497d6a77c611f476828fb8fe19a6a75cca2fa44cdab6bce1dc06b045764.md)

    Format with three components of 16-bit normalized unsigned integer. Supported only by .png. 

* [rgba16_unorm](group___image_1gga7facda497d6a77c611f476828fb8fe19a3b5f3e88d62e02ec478af8276857b13a.md)

    Format with four components of 16-bit normalized unsigned integer. Supported only by .png. 

* [r32_float](group___image_1gga7facda497d6a77c611f476828fb8fe19a883a4b0635de0ee0dcbee5e7c0c9f2c0.md)

    Format with one component of 32-bit floating-point number. Supported only by .hdr. 

* [rg32_float](group___image_1gga7facda497d6a77c611f476828fb8fe19a1bd20568b6cce706c8eafd4654d1370a.md)

    Format with two components of 32-bit floating-point number. Supported only by .hdr. 

* [rgb32_float](group___image_1gga7facda497d6a77c611f476828fb8fe19a66eaf1dc4f84217a7bbe1dc1ad5b3708.md)

    Format with three components of 32-bit floating-point number. Supported only by .hdr. 

* [rgba32_float](group___image_1gga7facda497d6a77c611f476828fb8fe19a3ed8a903f11738255bdc8928b5d9885c.md)

    Format with four components of 32-bit floating-point number. Supported only by .hdr. 

