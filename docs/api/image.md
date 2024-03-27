# Image
Image module provides functions to parse and save image files. 

## Topics
* [Image Errors](image_error.md)
## Types
* [Luna::Image::DDSImageDesc](struct_luna_1_1_image_1_1_d_d_s_image_desc.md)

    Describes one DDS image. 


* [Luna::Image::DDSSubresource](struct_luna_1_1_image_1_1_d_d_s_subresource.md)

    Describes one subresource in one DDS image. 


* [Luna::Image::DDSImage](struct_luna_1_1_image_1_1_d_d_s_image.md)

    Represents one loaded DDS image. 


* [Luna::Image::ImageDesc](struct_luna_1_1_image_1_1_image_desc.md)

    Describes one image file (except DDS, which is described by [DDSImageDesc](struct_luna_1_1_image_1_1_d_d_s_image_desc.md)). 


## Enumerations
* [Luna::Image::DDSFlag](group___image_1ga6786d47f5b6b295892428b360b53f0ec.md)

    Specifies additional flags of one DDS image. 

* [Luna::Image::DDSFormat](group___image_1gaadf6475eb5b53a62dfbde2a85e07bc25.md)

    Specifies pixel formats of one DDS image. Maps to DXGI_FORMAT. 

* [Luna::Image::DDSDimension](group___image_1ga2b7189cde25cf81d2d8d04a0f7197be0.md)

    Specifies the dimension of one DDS texture. 

* [Luna::Image::ImageFormat](group___image_1ga7facda497d6a77c611f476828fb8fe19.md)

    Formats that can be saved in one image file (except DDS, which is identified by [DDSFormat](group___image_1gaadf6475eb5b53a62dfbde2a85e07bc25.md)). 

## Functions
* [bool is_valid(DDSFormat fmt)](group___image_1ga300c2427280175ca0c6500ccc4dbb624.md)

    Checks whether one DDSFormat is a valid format for DDS files. 

* [bool is_compressed(DDSFormat fmt)](group___image_1ga29d80502eeb26645b2ca96706d346308.md)

    Checks whether one DDSFormat is a compressed format. 

* [bool is_packed(DDSFormat fmt)](group___image_1gad9c656b3c7127354aa86bf0ceb921bde.md)

    Checks whether one DDSFormat is a packed format. 

* [usize bits_per_pixel(DDSFormat fmt)](group___image_1ga1867055a65e999a325512439e70eacd8.md)

    Gets the number of bits used to represent one pixel in the specified format. 

* [constexpr u32 calc_dds_subresoruce_index(u32 mip_slice, u32 array_slice, u32 mip_levels)](group___image_1ga68aa43b300173227d7c7abea0303449f.md)

    Calculates subresource index for the specified subresource in DDS image. 

* [R< DDSImage > new_dds_image(const DDSImageDesc &desc)](group___image_1gaba122687af431e10eb7185a4b9ed533e.md)

    Creates one new DDS image object that can be saved later. 

* [R< DDSImageDesc > read_dds_image_file_desc(const void *data, usize data_size)](group___image_1ga15d27781a165f7cc81bc622bf92508b8.md)

    Reads DDS image description from DDS image file data. 

* [R< DDSImage > read_dds_image(const void *data, usize data_size)](group___image_1gaa6cd4b7739d2ff0374b56129fedd65d7.md)

    Reads DDS image data from DDS image file data. 

* [RV write_dds_file(ISeekableStream *stream, const DDSImage &image)](group___image_1ga0789e2039dce97a6cbbc95ec2b4024bc.md)

    Writes the DDS image to one DDS file. 

* [constexpr u32 pixel_size(ImageFormat format)](group___image_1gae7adcd2b70252a925680a35eeac22f89.md)

    Gets the size of one pixel of the specified format in bytes. 

* [R< ImageDesc > read_image_file_desc(const void *data, usize data_size)](group___image_1ga5a355cc8fb58136d5b8ba73acc373a2d.md)

    Reads image description from image file data. 

* [R< Blob > read_image_file(const void *data, usize data_size, ImageFormat desired_format, ImageDesc &out_desc)](group___image_1gacca121ce34e223f4799df774ec9e38c7.md)

    Reads image description and pixel data from image file data. 

* [RV write_png_file(ISeekableStream *stream, const ImageDesc &desc, const void *data, usize data_size)](group___image_1gaad6a6a99babe3fcdb9b57cbbf034dbe1.md)

    Writes the image data to one PNG file. 

* [RV write_bmp_file(ISeekableStream *stream, const ImageDesc &desc, const void *data, usize data_size)](group___image_1ga9b8ce0d86fd7a9fd8288da322640bc75.md)

    Writes the image data to one BMP file. 

* [RV write_tga_file(ISeekableStream *stream, const ImageDesc &desc, const void *data, usize data_size)](group___image_1ga3a0a7abb65096e2ccbce508b24ac689e.md)

    Writes the image data to one TGA file. 

* [RV write_jpg_file(ISeekableStream *stream, const ImageDesc &desc, const void *data, usize data_size, u32 quality)](group___image_1gaba4f480db40bf65eafafc90db5913f74.md)

    Writes the image data to one JPEG file. 

* [RV write_hdr_file(ISeekableStream *stream, const ImageDesc &desc, const void *data, usize data_size)](group___image_1ga453f9d6a9f8d83928a666856df7c5689.md)

    Writes the image data to one HDR file. 

* [Image::ImageFormat get_rhi_desired_format(Image::ImageFormat format)](group___image_1gac5f3c86e911e7f69aef3a6b934a4c99f.md)

    Gets desired image format form RHI format. 

* [RHI::Format image_to_rhi_format(Image::ImageFormat format)](group___image_1ga61ceadcd7d21f6816079cf16e3ec2a66.md)

    Converts image format to RHI format. 

* [Image::ImageFormat rhi_to_image_format(RHI::Format format)](group___image_1ga0fa74039631c5aead1cdf2e9dc080f2f.md)

    Converts RHI format to image format. 

* [RHI::Format dds_to_rhi_format(Image::DDSFormat format)](group___image_1ga8bb477a238818cd4225c7217cbf7170c.md)

    Converts DDS image format to RHI format. 

* [DDSFormat rhi_to_dds_format(RHI::Format format)](group___image_1ga0336592f2c1a8c472b95d8f34867dd90.md)

    Converts RHI format to DDS image format. 

