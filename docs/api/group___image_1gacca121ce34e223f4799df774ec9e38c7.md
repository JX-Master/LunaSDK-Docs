# Luna::Image::read_image_file

```c++
R< Blob > read_image_file(const void *data, usize data_size, ImageFormat desired_format, ImageDesc &out_desc)
```

Reads image description and pixel data from image file data. 



## Parameters
* *in* **data**

    The image file data. Image file formats are detected from data automatically. 

* *in* **data_size**

    The size of the image file data in bytes. 

* *in* **desired_format**

    The desired pixel format for data in the blob returned by this function. If this does not matches the actual format of the file, pixel format conversion will be performed automatically. 

* *out* **out_desc**

    The image description for the returned image data. 

## Return value
Returns one blob that contains the image pixel data. Pixels are arranged in row-major order, and there is no padding between every two rows of data. 

