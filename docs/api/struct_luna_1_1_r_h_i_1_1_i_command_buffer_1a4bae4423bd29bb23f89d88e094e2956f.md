# Luna::RHI::ICommandBuffer::copy_buffer_to_texture

```c++
virtual void copy_buffer_to_texture(ITexture *dst, SubresourceIndex dst_subresource, u32 dst_x, u32 dst_y, u32 dst_z, IBuffer *src, u64 src_offset, u32 src_row_pitch, u32 src_slice_pitch, u32 copy_width, u32 copy_height, u32 copy_depth)=0
```

Copies texture data region from one buffer to one texture. Texture data in the buffer is interpreted in row-major arrangement. 



## Parameters
* *in* **dst**

    The texture to copy data to. 

* *in* **dst_subresource**

    The subresource in `dst` to copy data to. 

* *in* **dst_x**

    The X position of the first pixel to copy data to. 

* *in* **dst_y**

    The Y position of the first pixel to copy data to. 

* *in* **dst_z**

    The Z position of the first pixel to copy data to. 

* *in* **src**

    The buffer to copy data from. 

* *in* **src_offset**

    The offset, in bytes, of the first pixel data to copy from in `src`. 

* *in* **src_row_pitch**

    The number of bytes to advance between every row of data in `src`. 

* *in* **src_slice_pitch**

    The number of bytes to advance between every slice (row * column) of data in `src`. 

* *in* **copy_width**

    The number of pixels to copy for each row. 

* *in* **copy_height**

    The number of rows to copy for each slice. 

* *in* **copy_depth**

    The number of slices to copy. 

