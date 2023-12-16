# Luna::Blob
Represents one binary large object (BLOB). 

```c++
class Luna::Blob
```

[Blob](class_luna_1_1_blob.md) can be used as a RAII wrapper for arbitrary memory allocation. One blob object allocates and manages one memory block that stores the blob data, which we call the "managed memory" of the blob object. The managed memory is always allocated from [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md) or [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md). The user can also allocate the memory manually then attach it to one blob object by calling Blob::attach, or call Blob::detach to take ownership of the managed memory from one blob object. 

