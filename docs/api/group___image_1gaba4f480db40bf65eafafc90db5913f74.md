# Luna::Image::write_jpg_file

```c++
RV write_jpg_file(ISeekableStream *stream, const ImageDesc &desc, const void *data, usize data_size, u32 quality)
```

Writes the image data to one JPEG file. 



## Parameters
* *in* **stream**

    The stream to write file data to. 

* *in* **desc**

    The image description. 

* *in* **data**

    The image pixel data. Pixels are arranged in row-major order, and there is no padding between every two rows of data. 

* *in* **data_size**

    The image pixel data size in bytes. 

* *in* **quality**

    The file compression quality. This value is between 1 and 100, higher quality looks better but results in a bigger image. 

