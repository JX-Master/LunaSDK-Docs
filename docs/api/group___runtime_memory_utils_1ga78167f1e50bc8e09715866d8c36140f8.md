# Luna::memcpy_bitmap

```c++
void * memcpy_bitmap(void *dst, const void *src, usize copy_size_per_row, usize num_rows, usize dst_row_pitch, usize src_row_pitch)
```

Copies the data for a 2D bitmap. 

## Overview


## Parameters
### dst
A pointer to the first pixel to be copied in destination bitmap. 

### src
A pointer to the first pixel to be copied in source bitmap. 

### copy_size_per_row
The size of the data to be copied for every row, in bytes. 

### num_rows
The number of rows to copy. 

### dst_row_pitch
The pitch to advance for one row in destination bitmap in bytes. 

### src_row_pitch
The pitch to advance for one row in source bitmap in bytes. 

## Return value
Returns the `dst` pointer. 

