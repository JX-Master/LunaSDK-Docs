# Luna::ISeekableStream::set_size

```c++
virtual RV set_size(u64 size)=0
```

Sets the size of the stream buffer. 

If the current stream buffer size is smaller than the size to set and this call succeeded, the stream buffer will be extended to the size specified, with data between the last size and current size be uninitialized. If the current stream buffer size is greater than the size to set and this call succeeded, the stream buffer will be truncated and the data between the last size and current size will be discarded. 

## Parameters
* *in* **size**

    The size to set, in bytes. 

