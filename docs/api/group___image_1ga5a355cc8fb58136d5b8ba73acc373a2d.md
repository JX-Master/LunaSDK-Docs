# Luna::Image::read_image_file_desc

```c++
R< ImageDesc > read_image_file_desc(const void *data, usize data_size)
```

Reads image description from image file data. 



## Parameters
* *in* **data**

    The image file data. Image file formats are detected from data automatically. 

* *in* **data_size**

    The size of the image file data in bytes. 

## Return value
Returns the image description. 

