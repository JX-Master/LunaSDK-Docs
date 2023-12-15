# Luna::IStream::read

```c++
virtual RV read(void *buffer, usize size, usize *read_bytes=nullptr)=0
```

Reads data from the current position the cursor is pointing to and offsets the cursor back. If the data to be read is not ready, the platform suspends the calling thread until the data is ready. 

## Parameters
### buffer
The buffer to accept the read data. 

### size
The size, in bytes, to read from the stream. 

### read_bytes
If not `nullptr`, the system sets the actual size of bytes being read to the buffer to this parameter. The actual size of bytes being read may be smaller than the size of bytes required to be read if the cursor reaches the end of the stream, but this is NOT an error. Specially, if one read operation is performed when the cursor is beyond or at the end of the stream, the read operation succeeds with 0 bytes being read. This can be considered as an EOF symbol in stdlib. 

