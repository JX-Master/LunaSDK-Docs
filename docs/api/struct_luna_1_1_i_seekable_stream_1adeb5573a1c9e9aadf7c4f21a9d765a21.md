# Luna::ISeekableStream::seek

```c++
virtual RV seek(i64 offset, SeekMode mode)=0
```

Moves the read/write cursor to a new position. 

## Overview


## Parameters
### offset
Number of bytes to move relative to the position specified by `mode`. 

### mode
The seek mode to use. 


The cursor value cannot be negative, if the new cursor position goes below 0, the seek operation fails. 

