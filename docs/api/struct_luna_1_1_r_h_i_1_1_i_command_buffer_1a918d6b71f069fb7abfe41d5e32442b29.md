# Luna::RHI::ICommandBuffer::copy_texture

```c++
virtual void copy_texture(ITexture *dst, SubresourceIndex dst_subresource, u32 dst_x, u32 dst_y, u32 dst_z, ITexture *src, SubresourceIndex src_subresource, u32 src_x, u32 src_y, u32 src_z, u32 copy_width, u32 copy_height, u32 copy_depth)=0
```

Copies texture data region from one texture to another. 



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

    The number of pixels to copy in X dimension. 

* *in* **copy_height**

    The number of pixels to copy in Y dimension. 

* *in* **copy_depth**

    The number of pixels to copy in Z dimension. 

