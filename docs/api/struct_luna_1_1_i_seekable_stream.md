# Luna::ISeekableStream
Represents one stream object that supports setting the cursor position. 

```c++
interface Luna::ISeekableStream : public virtual IStream
```

## Functions
* [virtual R< u64 > tell()=0](struct_luna_1_1_i_seekable_stream_1a62f27c4617444c74fd3c5e30fa146020.md)

    Gets the current position of the stream cursor. 

* [virtual RV seek(i64 offset, SeekMode mode)=0](struct_luna_1_1_i_seekable_stream_1adeb5573a1c9e9aadf7c4f21a9d765a21.md)

    Moves the read/write cursor to a new position. 

* [virtual u64 get_size()=0](struct_luna_1_1_i_seekable_stream_1a4dbeb603c9f042cd59f6c5e60f5deeaf.md)

    Gets the size of the stream buffer in bytes. 

* [virtual RV set_size(u64 size)=0](struct_luna_1_1_i_seekable_stream_1a2aa8f3bce4e55eacddc0a759319a6272.md)

    Sets the size of the stream buffer. 

