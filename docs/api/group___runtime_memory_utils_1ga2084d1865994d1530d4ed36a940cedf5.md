# Luna::memcpy_bitmap3d

```c++
void * memcpy_bitmap3d(void *dst, const void *src, usize copy_size_per_row, usize num_rows, usize num_slices, usize dst_row_pitch, usize src_row_pitch, usize dst_slice_pitch, usize src_slice_pitch)
```

Copies the data for a 3D bitmap. 



## Parameters
* *in* **dst**

    A pointer to the first pixel to be copied in destination bitmap. 

* *in* **src**

    A pointer to the first pixel to be copied in source bitmap. 

* *in* **copy_size_per_row**

    The size of the data to be copied for every row, in bytes. 

* *in* **num_rows**

    The number of rows to copy. 

* *in* **num_slices**

    The number of slices (layers) to copy. 

* *in* **dst_row_pitch**

    The pitch to advance for one row in destination bitmap in bytes. 

* *in* **src_row_pitch**

    The pitch to advance for one row in source bitmap in bytes. 

* *in* **dst_slice_pitch**

    The pitch to advance for one slice (layer) in destination bitmap in bytes. 

* *in* **src_slice_pitch**

    The pitch to advance for one slice (layer) in source bitmap in bytes. 

## Return value
Returns the `dst` pointer. 

