# Luna::pixel_offset

```c++
const void * pixel_offset(const void *base, usize x, usize y, usize z, usize bytes_per_pixel, usize row_pitch, usize slice_pitch)
```

Returns a pointer that offsets the specified pixels in the bitmap. 



## Parameters
* *in* **base**

    The pointer to the first pixel in the bitmap. 

* *in* **x**

    The x offset in pixels. 

* *in* **y**

    The y offset in pixels. 

* *in* **z**

    The z offset in pixels. 

* *in* **bytes_per_pixel**

    The number of bytes per pixel. 

* *in* **row_pitch**

    The pitch to advance for one row in bytes. 

* *in* **slice_pitch**

    The pitch to advance for one slice in bytes. 

## Return value
Returns the offseted pointer. 

