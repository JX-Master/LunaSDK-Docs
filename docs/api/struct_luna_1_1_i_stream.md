# Luna::IStream
Represents a serial stream sequence of bytes and supports read/write operations on them. 

```c++
interface Luna::IStream : public virtual Interface
```

## Overview
Common implementations of streams include file, memory buffer, web socket and so on.

This object is not thread safe and the I/O operations on this object is not asynchronous (will suspend the current thread until the operation is done or failed). 

## Functions
* [virtual RV read(void *buffer, usize size, usize *read_bytes=nullptr)=0](struct_luna_1_1_i_stream_1a6a5956c629eb0bba95dc0dd89bd0abde.md)
* [virtual RV write(const void *buffer, usize size, usize *write_bytes=nullptr)=0](struct_luna_1_1_i_stream_1ae2de26864471bdff2d8f7d49ac47da39.md)
