# Luna::IStream::write

```c++
virtual RV write(const void *buffer, usize size, usize *write_bytes=nullptr)=0
```

## Overview
Writes data to the current position the cursor is pointing to and offsets the cursor back. This call returns after all data have been written. 

## Parameters
### buffer
The buffer that holds the data to be written. 

### size
The size, in bytes, to write to the stream. 

### write_bytes
If not `nullptr`, the system sets the actual size of bytes being written to this parameter. Mostly, if the cursor goes beyond the end of the stream buffer while writing data, the stream will be expanded so the succeeding data can be written, so unless an error occurs, the size of bytes written will always equal to the size of bytes required by the user to write. However, if an error occurs while writing data, some of the data may have already be written while others are not, in such case the `write_bytes` reported by system may not be equal to `size` specified by the user. 

