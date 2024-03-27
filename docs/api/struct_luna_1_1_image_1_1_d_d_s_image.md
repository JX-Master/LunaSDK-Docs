# Luna::Image::DDSImage
Represents one loaded DDS image. 

```c++
struct Luna::Image::DDSImage
```

Do not initialize this object by yourself, instead, creates one empty DDS image object by calling [new_dds_image](group___image_1gaba122687af431e10eb7185a4b9ed533e.md), which will allocate pixel memory and initialize subresource descriptors 

## Member objects
* [DDSImageDesc desc](struct_luna_1_1_image_1_1_d_d_s_image_1a5a1b3f52b015eaab7dd81e39a6a937ec.md)

    The image descriptor. 

* [Blob data](struct_luna_1_1_image_1_1_d_d_s_image_1a7c23772f64dee4d38b5be05282b2e321.md)

    The image pixel data. 

* [Array<DDSSubresource> subresources](struct_luna_1_1_image_1_1_d_d_s_image_1a150fb03b704c0596e29f7b799efad3bd.md)

    An array of subresource descriptors. 

