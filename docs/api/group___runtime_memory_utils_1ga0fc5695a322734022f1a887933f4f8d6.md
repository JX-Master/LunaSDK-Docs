# Luna::pixel_offset

```c++
void * pixel_offset(void *base, usize x, usize y, usize z, usize bytes_per_pixel, usize row_pitch, usize slice_pitch)
```

Returns a pointer that offsets the specified pixels in the bitmap. 

## Overview


## Parameters
### base
The pointer to the first pixel in the bitmap. 

### x
The x offset in pixels. 

### y
The y offset in pixels. 

### z
The z offset in pixels. 

### bytes_per_pixel
The number of bytes per pixel. 

### row_pitch
The pitch to advance for one row in bytes. 

### slice_pitch
The pitch to advance for one slice in bytes. 

## Return value
Returns the offseted pointer. 

