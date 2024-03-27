# Luna::Image::write_tga_file

```c++
RV write_tga_file(ISeekableStream *stream, const ImageDesc &desc, const void *data, usize data_size)
```

Writes the image data to one TGA file. 



## Parameters
* *in* **stream**

    The stream to write file data to. 

* *in* **desc**

    The image description. 

* *in* **data**

    The image pixel data. Pixels are arranged in row-major order, and there is no padding between every two rows of data. 

* *in* **data_size**

    The image pixel data size in bytes. 

