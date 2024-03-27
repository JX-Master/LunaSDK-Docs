# Luna::Image::rhi_to_image_format

```c++
Image::ImageFormat rhi_to_image_format(RHI::Format format)
```

Converts RHI format to image format. 



## Parameters
* *in* **format**

    The RHI format. 

## Return value
Returns the converted image format. Returns [ImageFormat::unknown](group___image_1gga7facda497d6a77c611f476828fb8fe19aad921d60486366258809553a3db49a4a.md) if no image format can be mapped to the specified RHI format. 

