# Luna::Image::new_dds_image

```c++
R< DDSImage > new_dds_image(const DDSImageDesc &desc)
```

Creates one new DDS image object that can be saved later. 



## Parameters
* *in* **desc**

    The DDS image descriptor. 

## Return value
Returns the created DDS image. The pixel memory of the returned DDS image is allocated but uninitialized, the user should fill the pixel data by itself. 

