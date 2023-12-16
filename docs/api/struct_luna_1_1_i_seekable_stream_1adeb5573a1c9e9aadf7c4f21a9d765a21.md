# Luna::ISeekableStream::seek

```c++
virtual RV seek(i64 offset, SeekMode mode)=0
```

Moves the read/write cursor to a new position. 



## Parameters
* *in* **offset**

    Number of bytes to move relative to the position specified by `mode`. 

* *in* **mode**

    The seek mode to use. 

## Remark
The cursor position is not bound to the size of the stream. If you move the cursor beyond the end of the stream, the cursor is still valid with the following behaviors:1. All read operations succeed with 0 byte being read, just like EOF behaviors.

1. All write operations extends the size of the stream before the actual write operation performed.


The cursor value cannot be negative, if the new cursor position goes below 0, the seek operation fails. 

