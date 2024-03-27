# Luna::RHI::ICommandBuffer::copy_texture_to_buffer

```c++
virtual void copy_texture_to_buffer(IBuffer *dst, u64 dst_offset, u32 dst_row_pitch, u32 dst_slice_pitch, ITexture *src, SubresourceIndex src_subresource, u32 src_x, u32 src_y, u32 src_z, u32 copy_width, u32 copy_height, u32 copy_depth)=0
```

Copies texture data region from one texture to one buffer. Texture data is written to the buffer in row-major arrangement. 



## Parameters
* *in* **dst**

    The buffer to copy data to. 

* *in* **dst_offset**

    The offset, in bytes, of the first data byte to copy data to in `dst`. 

* *in* **dst_row_pitch**

    The number of bytes to advance between every row of data in `dst`. 

* *in* **dst_slice_pitch**

    The number of bytes to advance between every slice (row * column) of data in `dst`. 

* *in* **src**

    The texture to copy data from. 

* *in* **src_subresource**

    The subresource in `src` to copy data from. 

* *in* **src_x**

    The X position of the first pixel to copy data from. 

* *in* **src_y**

    The Y position of the first pixel to copy data from. 

* *in* **src_z**

    The Z position of the first pixel to copy data from. 

* *in* **copy_width**

    The number of pixels to copy for each row. 

* *in* **copy_height**

    The number of rows to copy for each slice. 

* *in* **copy_depth**

    The number of slices to copy. 

