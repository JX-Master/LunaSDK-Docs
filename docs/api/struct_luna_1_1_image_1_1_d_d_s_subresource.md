# Luna::Image::DDSSubresource
Describes one subresource in one DDS image. 

```c++
struct Luna::Image::DDSSubresource
```

## Member objects
* [u32 width](struct_luna_1_1_image_1_1_d_d_s_subresource_1a85db88ffee2944ecd35c616393976289.md)

    The width of this subresource in pixels. 

* [u32 height](struct_luna_1_1_image_1_1_d_d_s_subresource_1add40f8a56ae8cc650f92a3aa4d2bac99.md)

    The height of this subresource in pixels. 

* [u32 depth](struct_luna_1_1_image_1_1_d_d_s_subresource_1aebf034dca5d4441f3b12bc2aaa9af93c.md)

    The depth of this subresource in pixels. 

* [usize row_pitch](struct_luna_1_1_image_1_1_d_d_s_subresource_1a1ddf650da937268b82fd27981c664725.md)

    The number of bytes to advance between every two rows of data of this subresource. 

* [usize slice_pitch](struct_luna_1_1_image_1_1_d_d_s_subresource_1aff52acd056cb03f33beb8f32bcebd180.md)

    The number of bytes to advance between every two slices (rows * columns) of data of this subresource. 

* [usize data_offset](struct_luna_1_1_image_1_1_d_d_s_subresource_1a48eb3f8a1040527020ce7898c7936655.md)

    The offset, in bytes, of the beginning data of this subresource from the beginning of the image pixel data. 

